<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>BBB Transport — Computational Modeling</title>
  <link rel="stylesheet" href="styles.css" />
  <meta name="description" content="Computational modeling and ML-driven predictions for drug transport across the blood–brain barrier." />
</head>
<body>
  <header class="navwrap">
    <div class="container">
      <h1 class="brand">BBB Transport — Computational Modeling</h1>
      <nav class="mainnav">
        <a href="index.html">Home</a>
        <a href="about.html">Research Plan</a>
        <a href="methods.html">Methods & Results</a>
        <a href="simulate.html">Interactive Simulator</a>
        <a href="poster.html">Poster & Files</a>
        <a href="contact.html">Contact</a>
      </nav>
    </div>
  </header>

  <main class="container hero">
    <section class="intro card">
      <h2>Bridging molecular design and transport behavior</h2>
      <p class="lead">Our research creates a predictive computational framework to model, simulate, and optimize transport across the blood–brain barrier (BBB). We combine deterministic kinetic models, stochastic diffusion simulations, and machine learning-driven molecular feature analysis to accelerate rational design of therapeutic vectors that can reach the CNS.</p>

      <div class="cta-row">
        <a class="btn" href="simulate.html">Try the Simulator</a>
        <a class="btn ghost" href="poster.html">Open Poster</a>
      </div>
    </section>

    <section class="cards grid-3">
      <div class="card">
        <h3>Intellectual Merit</h3>
        <p>Mechanistic modeling + ML feature selection to reveal design principles that increase permeability across BBB-like interfaces.</p>
      </div>
      <div class="card">
        <h3>Broader Impacts</h3>
        <p>Open-source tools for education and translational research. Classroom-ready interactive simulations allow students to visualize how design changes affect transport.</p>
      </div>
      <div class="card">
        <h3>Applications</h3>
        <ul>
          <li>CNS drug development guidance</li>
          <li>Predictive screening of nanoparticle features</li>
          <li>Education and reproducible research</li>
        </ul>
      </div>
    </section>

    <section class="card highlight">
      <h2>Quick highlights</h2>
      <div class="kpis">
        <div class="kpi"><strong>120+</strong><span>Model runs</span></div>
        <div class="kpi"><strong>1M+</strong><span>Simulated particles</span></div>
        <div class="kpi"><strong>Open-source</strong><span>Planned release</span></div>
      </div>
    </section>
  </main>

  <footer class="footer">
    <div class="container">
      <small>Poster: <code>/mnt/data/Quant2 Final Poster.pdf</code> — Notebook: <code>/mnt/data/Final Project (1).ipynb</code></small>
      <p>© 2025 Alex — Computational Modeling of BBB transport</p>
    </div>
  </footer>
</body>
</html>

:root{
  --bg:#f5f7fb; --card:#fff; --accent:#0b5fff; --muted:#334155;
  --glass: rgba(255,255,255,0.7);
}
*{box-sizing:border-box}
body{font-family:Inter,system-ui,Segoe UI,Roboto,Arial,sans-serif;margin:0;background:var(--bg);color:var(--muted);-webkit-font-smoothing:antialiased}
.container{max-width:1100px;margin:0 auto;padding:20px}
.navwrap{background:linear-gradient(90deg,#0b5fff16,#0b5fff06);border-bottom:1px solid #e6ecff}
.brand{display:flex;align-items:center;gap:14px}
.brand img{height:44px}
.brand h1{margin:8px 0;color:#062a7c;font-size:20px}
.mainnav{margin-top:6px}
.mainnav a{margin-right:16px;color:var(--accent);text-decoration:none;font-weight:600}
.hero{padding:40px 20px}
.lead{font-size:18px;color:#1f2937}
.grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:18px;margin-top:18px}
.card{background:var(--card);padding:18px;border-radius:12px;box-shadow:0 6px 18px rgba(15,23,42,0.06)}
.highlight{margin-top:18px}
.btn{display:inline-block;padding:10px 14px;border-radius:10px;background:var(--accent);color:white;text-decoration:none;font-weight:700;margin-right:8px}
.btn.ghost{background:transparent;color:var(--accent);border:2px solid var(--accent)}
.kpis{display:flex;gap:12px}
.kpi{background:linear-gradient(180deg,#fbfdff,#f7fbff);padding:10px;border-radius:10px;min-width:120px;text-align:center}
.footer{padding:24px 20px;text-align:center;color:#889}
@media (max-width:900px){
  .grid-3{grid-template-columns:1fr}
  .brand h1{font-size:18px}
}

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Research Plan — BBB Transport</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="navwrap">
    <div class="container">
      <h1 class="brand">Research Plan — BBB Transport</h1>
      <nav class="mainnav">
        <a href="index.html">Home</a>
        <a href="about.html">Research Plan</a>
        <a href="methods.html">Methods</a>
        <a href="simulate.html">Simulator</a>
        <a href="poster.html">Poster</a>
      </nav>
    </div>
  </header>

  <main class="container">
    <article class="card">
      <h2>Graduate Research Plan Statement</h2>
      <p>The impermeable nature of the blood–brain barrier (BBB) remains a major hurdle for treating neurological diseases. Despite major advances in drug design, over 98% of small molecules fail to reach therapeutic concentrations in the brain. Our proposed research aims to develop a computational framework for simulating and optimizing drug delivery strategies that enable efficient and selective transport across the BBB.</p>

      <h3>Project overview</h3>
      <p>The proposed research seeks to analyze the many factors that influence the diffusion of particles across the blood–brain barrier (BBB). The BBB’s selectivity remains one of the greatest challenges in neuroscience, pharmaceutical delivery, and biomaterials design. By quantifying and modeling the diffusion coefficients of both nanoparticles and biologically derived molecules with varying size, charge, and surface chemistry, this project will provide insights into how molecular transport is controlled by various microenvironments.</p>

      <h3>Approach</h3>
      <p>This project will integrate computational modeling, biophysical properties, and experimental datasets. Using imaging and stochastic diffusion models, it will bridge the gap between molecular interactions and transport behavior. Through this research, we aim to develop consistent modeling, experimental data for transport kinetics, and information regarding barrier responsiveness.</p>

      <h3>Intellectual Merit</h3>
      <p>The objective is to develop a predictive, mechanistic framework for drug transport across the BBB applying pharmacology, molecular transport modeling, and machine learning. Differential equations, stochastic models and ML identify molecular features correlated with permeability. Interdisciplinary work engages neurobiology, chemical engineering, biomaterials, and computation.</p>

      <h3>Broader Impacts</h3>
      <p>Findings will accelerate CNS therapy development, provide classroom-ready interactive tools, and be shared as open-source software. The platform is designed for modular educational use so students worldwide can visualize how molecular design influences BBB transport.</p>
    </article>
  </main>

  <footer class="footer"><div class="container">© 2025 Alex — BBB Transport</div></footer>
</body>
</html>

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Methods & Results — BBB Transport</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="navwrap">
    <div class="container"><h1 class="brand">Methods & Results</h1>
      <nav class="mainnav">
        <a href="index.html">Home</a>
        <a href="about.html">Research Plan</a>
        <a href="methods.html">Methods</a>
        <a href="simulate.html">Simulator</a>
      </nav>
    </div>
  </header>

  <main class="container">
    <section class="card">
      <h2>Modeling framework</h2>
      <p>We combine three computational pillars:</p>
      <ol>
        <li><strong>Deterministic compartmental models:</strong> ODEs describing transcytosis, paracellular leakage, and clearance.</li>
        <li><strong>Stochastic particle simulations:</strong> Brownian/sub-diffusive trajectories to capture heterogeneity and rare crossing events.</li>
        <li><strong>Machine learning:</strong> Feature selection and supervised regression to predict permeability from molecular descriptors.</li>
      </ol>

      <h3>Example results (summary)</h3>
      <ul>
        <li>Smaller particles (<80 nm) with neutral-to-moderate positive charge and amphiphilic patches showed improved crossing probabilities in simulations.</li>
        <li>Simulated trends aligned with literature: receptor-mediated strategies outperform passive diffusion for large biologics.</li>
        <li>ML feature importance highlighted size, charge distribution, and hydrophobic surface fraction as top predictors.</li>
      </ul>

      <h3>Where the data come from</h3>
      <p>We integrate published experimental kinetics, imaging-derived permeability datasets, and internal simulations. The final site will link to our code repository and datasets for reproducible research.</p>
    </section>
  </main>

  <footer class="footer"><div class="container">© 2025 Alex — Methods</div></footer>
</body>
</html>

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Poster & Project Files</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="navwrap"><div class="container"><h1 class="brand">Poster & Files</h1>
    <nav class="mainnav"><a href="index.html">Home</a><a href="simulate.html">Simulator</a></nav>
  </div></header>

  <main class="container">
    <section class="card">
      <h2>Final Project Poster</h2>
      <p>Click to open or download the poster. If you host this site on GitHub Pages, upload <code>Quant2 Final Poster.pdf</code> to the repository root and the links below will work.</p>
      <p><a class="btn" href="/mnt/data/Quant2 Final Poster.pdf" target="_blank">Open Poster PDF</a></p>
      <div style="margin-top:18px;">
        <h3>Final Project Notebook</h3>
        <p>Interactive analysis code and results are available in the notebook below. Upload <code>Final Project (1).ipynb</code> to the repo root for direct download.</p>
        <p><a class="btn ghost" href="/mnt/data/Final Project (1).ipynb" target="_blank">Download Notebook</a></p>
      </div>
    </section>
  </main>

  <footer class="footer"><div class="container">© 2025 Alex — Poster</div></footer>
</body>
</html>

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Contact — BBB Transport</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="navwrap"><div class="container"><h1 class="brand">Contact</h1>
    <nav class="mainnav"><a href="index.html">Home</a><a href="poster.html">Poster</a></nav></div></header>

  <main class="container">
    <section class="card">
      <h2>Reach out</h2>
      <p><strong>Lead:</strong> Alex — Computational & Biomaterials Modeling</p>
      <p>Email: <a href="mailto:alex@example.edu">alex@example.edu</a></p>
      <p>Want the code or to collaborate? Mention the project title: <em>Computational Modeling of Drug Transport Across the BBB</em>.</p>
    </section>
  </main>

  <footer class="footer"><div class="container">© 2025 Alex — Contact</div></footer>
</body>
</html>

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Interactive BBB Simulator</title>
  <link rel="stylesheet" href="styles.css" />
  <style>
    .sim-wrap{display:grid;grid-template-columns:1fr 320px;gap:18px;margin-top:18px}
    canvas{width:100%;height:420px;background:linear-gradient(180deg,#ffffff,#f3f6ff);border-radius:12px;display:block}
    .controls{position:relative}
    .control{margin-bottom:12px}
    label{display:block;margin-bottom:6px;font-weight:600;color:#223}
    .tiny{font-size:13px;color:#6b7280}
    .metric {background:#fff;padding:10px;border-radius:10px;box-shadow:0 6px 14px rgba(10,15,40,0.04);margin-bottom:12px}
  </style>
</head>
<body>
  <header class="navwrap"><div class="container"><h1 class="brand">Interactive Simulator</h1>
    <nav class="mainnav"><a href="index.html">Home</a><a href="simulate.html">Simulator</a><a href="methods.html">Methods</a></nav></div></header>

  <main class="container">
    <section class="card">
      <h2>Particle diffusion & barrier crossing demo</h2>
      <p class="tiny">This interactive demo visualizes Brownian-like particle motion in a 2D domain with a vertical "BBB" barrier. Adjust particle size, diffusion coefficient, and barrier permeability to see how crossing probability changes. This is an educational simplified model — for research-grade simulations use the full pipeline.</p>

      <div class="sim-wrap">
        <div>
          <canvas id="simCanvas" width="800" height="420"></canvas>
          <div style="margin-top:12px;display:flex;gap:12px">
            <button id="startBtn" class="btn">Start</button>
            <button id="resetBtn" class="btn ghost">Reset</button>
            <div style="flex:1" class="metric"><strong>Crossed:</strong> <span id="crossed">0</span> / <span id="total">0</span></div>
          </div>
        </div>

        <aside class="card controls">
          <div class="control">
            <label>Particle count: <span id="pcountLabel">500</span></label>
            <input id="pcount" type="range" min="50" max="2000" value="500" />
          </div>

          <div class="control">
            <label>Particle radius (nm): <span id="radiusLabel">40</span></label>
            <input id="radius" type="range" min="5" max="200" value="40" />
            <div class="tiny">(Smaller particles generally diffuse faster.)</div>
          </div>

          <div class="control">
            <label>Diffusion coefficient (D, μm²/s): <span id="dLabel">5</span></label>
            <input id="D" type="range" min="0.5" max="12" step="0.1" value="5" />
          </div>

          <div class="control">
            <label>Barrier permeability (0–1): <span id="permLabel">0.06</span></label>
            <input id="perm" type="range" min="0" max="1" step="0.01" value="0.06" />
            <div class="tiny">Higher = easier crossing when particles interact with barrier pores/receptors.</div>
          </div>

          <div class="control">
            <label>Charge (illustrative):</label>
            <select id="charge">
              <option value="neutral">Neutral</option>
              <option value="positive">Slightly positive</option>
              <option value="negative">Slightly negative</option>
            </select>
          </div>

          <div class="control">
            <div class="tiny">Tip: increase D and permeability to see more crossing events. Try varying particle radius and observe trend.</div>
          </div>
        </aside>
      </div>
    </section>
  </main>

  <footer class="footer"><div class="container">© 2025 Alex — Interactive Simulator</div></footer>

  <script>
  // Simple diffusion + barrier crossing demo
  const canvas = document.getElementById('simCanvas');
  const ctx = canvas.getContext('2d');
  const DPR = window.devicePixelRatio || 1;
  canvas.width = canvas.clientWidth * DPR;
  canvas.height = canvas.clientHeight * DPR;
  ctx.scale(DPR, DPR);

  const startBtn = document.getElementById('startBtn');
  const resetBtn = document.getElementById('resetBtn');
  const pcountSlider = document.getElementById('pcount');
  const radiusSlider = document.getElementById('radius');
  const DSlider = document.getElementById('D');
  const permSlider = document.getElementById('perm');
  const chargeSelect = document.getElementById('charge');

  const pcountLabel = document.getElementById('pcountLabel');
  const radiusLabel = document.getElementById('radiusLabel');
  const dLabel = document.getElementById('dLabel');
  const permLabel = document.getElementById('permLabel');
  const crossedEl = document.getElementById('crossed');
  const totalEl = document.getElementById('total');

  let particles = [];
  let running = false;
  let crossed = 0, totalLaunched=0;

  function rand(a,b){return a + Math.random()*(b-a);}

  function setupParticles(){
    particles = [];
    crossed = 0;
    totalLaunched = +pcountSlider.value;
    for(let i=0;i<totalLaunched;i++){
      particles.push({
        x: rand(10, canvas.clientWidth/2 - 20),
        y: rand(10, canvas.clientHeight-10),
        vx: 0, vy: 0,
        alive: true,
        crossed: false
      });
    }
    crossedEl.textContent = crossed;
    totalEl.textContent = totalLaunched;
  }

  function drawBackground(){
    ctx.clearRect(0,0,canvas.clientWidth, canvas.clientHeight);
    // draw left and right regions
    ctx.fillStyle = '#f8fafc';
    ctx.fillRect(0,0,canvas.clientWidth, canvas.clientHeight);
    // barrier (vertical)
    const bx = canvas.clientWidth/2;
    ctx.fillStyle = '#062a7c';
    ctx.fillRect(bx-3, 0, 6, canvas.clientHeight);
    // little pores drawn as lighter spots (visual)
    for(let i=0;i<10;i++){
      const py = (i+0.5)*canvas.clientHeight/10;
      ctx.fillStyle = 'rgba(255,255,255,0.06)';
      ctx.beginPath();
      ctx.arc(bx, py, 18, 0, Math.PI*2);
      ctx.fill();
    }
    // labels
    ctx.fillStyle = '#223';
    ctx.font = '13px system-ui, Arial';
    ctx.fillText('Bloodstream (inlet)', 12, 18);
    ctx.fillText('Brain (target)', canvas.clientWidth - 140, 18);
  }

  function step(dt){
    const radius = +radiusSlider.value;
    const D = +DSlider.value; // um^2/s
    // Convert D to pixel step variance: map domain size to approx physical scale (arbitrary mapping for visuals)
    // We'll scale so D in [0.5,12] produces reasonable motion.
    const scale = 0.7;
    const sigma = Math.sqrt(2 * D * dt) * scale;

    const perm = +permSlider.value;
    const charge = chargeSelect.value;

    for(const p of particles){
      if(!p.alive) continue;
      // random displacement
      p.x += rand(-1,1) * sigma * 10;
      p.y += rand(-1,1) * sigma * 10;

      // reflect off top/bottom
      if(p.y < 6) p.y = 6;
      if(p.y > canvas.clientHeight - 6) p.y = canvas.clientHeight - 6;

      // soft bias toward barrier for positive charge (illustrative)
      if(charge === 'positive'){
        p.x += 0.02 * sigma * 8;
      } else if(charge === 'negative'){
        p.x -= 0.02 * sigma * 8;
      }

      // if hits barrier line
      const bx = canvas.clientWidth/2;
      if(p.x + radius >= bx - 3 && !p.crossed){
        // crossing probability depends on permeability, particle size: bigger = less probable
        const sizeFactor = Math.max(0.01, 1 - (radius / 200)); // 0.01..1
        const prob = perm * sizeFactor;
        // small stochastic check: simulate receptor-mediated 'capture' with increased prob if positive charge
        let adjustedProb = prob;
        if(charge === 'positive') adjustedProb *= 1.6;
        if(Math.random() < adjustedProb){
          // crosses: teleport slightly into brain side and mark
          p.x = bx + 8 + Math.random() * 50;
          p.crossed = true;
          crossed++;
          p.alive = true; // still visible after crossing
        } else {
          // reflect
          p.x = bx - (radius + 8);
          p.vx *= -0.5;
        }
      }

      // keep particles within left region (don't let them start beyond)
      if(p.x < 6) p.x = 6;
      if(p.x > canvas.clientWidth - 6) p.x = canvas.clientWidth - 6;
    }
    crossedEl.textContent = crossed;
  }

  function render(){
    drawBackground();
    // draw particles
    const radius = +radiusSlider.value;
    for(const p of particles){
      ctx.beginPath();
      const col = p.crossed ? 'rgba(11,95,255,0.9)' : 'rgba(10,90,180,0.85)';
      ctx.fillStyle = col;
      ctx.arc(p.x, p.y, Math.max(2, radius/20), 0, Math.PI*2);
      ctx.fill();
    }
  }

  let last = performance.now();
  function loop(t){
    if(!running) return;
    const dt = (t - last)/1000; // seconds
    last = t;
    // cap step
    const stepDt = Math.min(dt, 0.05);
    step(stepDt);
    render();
    requestAnimationFrame(loop);
  }

  // controls
  pcountSlider.addEventListener('input', ()=>{ pcountLabel.textContent = pcountSlider.value; });
  radiusSlider.addEventListener('input', ()=>{ radiusLabel.textContent = radiusSlider.value; });
  DSlider.addEventListener('input', ()=>{ dLabel.textContent = DSlider.value; });
  permSlider.addEventListener('input', ()=>{ permLabel.textContent = permSlider.value; });

  startBtn.addEventListener('click', ()=>{
    if(!running){
      setupParticles();
      running = true;
      last = performance.now();
      requestAnimationFrame(loop);
      startBtn.textContent = 'Pause';
    } else {
      running = false;
      startBtn.textContent = 'Resume';
    }
  });

  resetBtn.addEventListener('click', ()=>{
    running = false;
    startBtn.textContent = 'Start';
    setupParticles();
    drawBackground();
    render();
  });

  // initial
  setupParticles();
  drawBackground();
  render();

  // responsive redraw on resize
  window.addEventListener('resize', ()=> {
    canvas.width = canvas.clientWidth * DPR;
    canvas.height = canvas.clientHeight * DPR;
    ctx.setTransform(DPR,0,0,DPR,0,0);
    drawBackground();
    render();
  });
  </script>
</body>
</html>
