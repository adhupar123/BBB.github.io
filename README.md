<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>BBB Transport — Interactive Simulation & Poster</title>

<style>
/* ----- BASIC STYLING ----- */
body{
  font-family: Arial, sans-serif;
  background:#f5f7fb;
  margin:0;
  padding:0;
  color:#223;
}
header{
  background:#0b5fff15;
  padding:18px;
  text-align:center;
  border-bottom:1px solid #dce6ff;
}
h1{margin:0;font-size:22px;color:#062a7c;}
.container{max-width:900px;margin:0 auto;padding:20px;}
.card{
  background:white;
  padding:20px;
  border-radius:12px;
  box-shadow:0 4px 16px rgba(0,0,0,0.06);
  margin-bottom:20px;
}
.btn{
  display:inline-block;
  padding:10px 14px;
  border-radius:10px;
  background:#0b5fff;
  color:white;
  text-decoration:none;
  font-weight:bold;
  margin:4px 2px;
}
.btn.ghost{
  background:white;
  border:2px solid #0b5fff;
  color:#0b5fff;
}

/* ----- SIMULATOR ----- */
#simCanvas{
  background:white;
  width:100%;
  height:380px;
  border:1px solid #ccd6ff;
  border-radius:10px;
}
label{font-weight:bold;}
input[type=range]{width:100%;}
.small{font-size:13px;color:#6b7280;}
</style>
</head>

<body>
<header>
  <h1>BBB Transport — Simulation + Poster</h1>
</header>

<div class="container">

  <!-- INTRO CARD -->
  <div class="card">
    <h2>Project Resources</h2>
    <p>Below are direct links to the project poster and computational notebook.</p>

    <!-- TODO: Replace these with your real URLs -->
    <a class="btn" href="CHANGE_ME_TO_PUBLIC_URL/Quant2_Final_Poster.pdf" target="_blank">Open Poster PDF</a>
    <a class="btn ghost" href="CHANGE_ME_TO_PUBLIC_URL/Final_Project_1.ipynb" target="_blank">Download Notebook</a>

    <p class="small">
      Upload your files to Google Drive → Right-click → “Get link” → set to “Anyone with link” → paste above.
    </p>
  </div>

  <!-- SIMULATOR CARD -->
  <div class="card">
    <h2>Interactive BBB Diffusion Simulator</h2>
    <p class="small">
      Adjust particle properties and watch diffusion + barrier crossing. This is a simplified educational model.
    </p>

    <canvas id="simCanvas"></canvas>

    <!-- Controls -->
    <div style="margin-top:16px">
      <label>Particle count: <span id="countLabel">500</span></label>
      <input id="countSlider" type="range" min="100" max="2000" value="500">

      <label>Particle radius (nm): <span id="radLabel">40</span></label>
      <input id="radSlider" type="range" min="5" max="150" value="40">

      <label>Diffusion D (μm²/s): <span id="dLabel">5</span></label>
      <input id="dSlider" type="range" min="0.5" max="12" step="0.1" value="5">

      <label>Barrier permeability (0–1): <span id="permLabel">0.05</span></label>
      <input id="permSlider" type="range" min="0" max="1" step="0.01" value="0.05">

      <button id="startBtn" class="btn" style="margin-top:10px">Start</button>
      <button id="resetBtn" class="btn ghost" style="margin-top:10px">Reset</button>
    </div>

    <p class="small">
      Crossed: <span id="crossed">0</span> / <span id="total">0</span>
    </p>
  </div>

</div>

<script>
/*********************************************************
 BASIC SIMULATOR — Cleaned & Simplified
**********************************************************/
const canvas = document.getElementById("simCanvas");
const ctx = canvas.getContext("2d");
canvas.width = canvas.clientWidth;
canvas.height = canvas.clientHeight;

let particles = [];
let running = false;
let crossed = 0;

function rand(a,b){return a + Math.random()*(b-a);}

function initParticles(){
  particles = [];
  crossed = 0;

  const N = +document.getElementById("countSlider").value;
  const r = +document.getElementById("radSlider").value/20;

  for(let i=0;i<N;i++){
    particles.push({
      x: rand(10, canvas.width/2 - 25),
      y: rand(10, canvas.height - 10),
      crossed:false,
      r:r
    });
  }
  document.getElementById("crossed").textContent = crossed;
  document.getElementById("total").textContent = N;
}

function drawBackground(){
  ctx.fillStyle = "white";
  ctx.fillRect(0,0,canvas.width,canvas.height);

  // barrier line
  ctx.fillStyle = "#0b5fff";
  ctx.fillRect(canvas.width/2 - 2, 0, 4, canvas.height);
}

function step(dt){
  const D = +document.getElementById("dSlider").value;
  const perm = +document.getElementById("permSlider").value;

  for(const p of particles){
    // random walk
    p.x += rand(-1,1) * D * dt * 20;
    p.y += rand(-1,1) * D * dt * 20;

    // boundaries
    if(p.y<5) p.y=5;
    if(p.y>canvas.height-5) p.y=canvas.height-5;

    // barrier check
    const bx = canvas.width/2;
    if(!p.crossed && p.x > bx - 5){
      if(Math.random() < perm){
        p.crossed = true;
        crossed++;
      } else {
        p.x = bx - 10;
      }
    }
  }
  document.getElementById("crossed").textContent = crossed;
}

function render(){
  drawBackground();
  for(const p of particles){
    ctx.beginPath();
    ctx.fillStyle = p.crossed ? "#0b5fff" : "#1e88e5";
    ctx.arc(p.x, p.y, p.r, 0, Math.PI*2);
    ctx.fill();
  }
}

let last = null;
function loop(t){
  if(!running) return;
  if(!last) last = t;
  const dt = (t-last)/1000;
  last = t;

  step(dt);
  render();
  requestAnimationFrame(loop);
}

/*** UI wiring ***/
document.getElementById("startBtn").onclick = ()=>{
  running = true;
  last = null;
  if(particles.length===0) initParticles();
  requestAnimationFrame(loop);
};
document.getElementById("resetBtn").onclick = ()=>{
  running = false;
  initParticles();
  drawBackground();
  render();
};

/*** labels ***/
document.getElementById("countSlider").oninput = e =>
  document.getElementById("countLabel").textContent=e.target.value;
document.getElementById("radSlider").oninput = e =>
  document.getElementById("radLabel").textContent=e.target.value;
document.getElementById("dSlider").oninput = e =>
  document.getElementById("dLabel").textContent=e.target.value;
document.getElementById("permSlider").oninput = e =>
  document.getElementById("permLabel").textContent=e.target.value;

/*** initial ***/
initParticles();
drawBackground();
render();
</script>

</body>
</html>
