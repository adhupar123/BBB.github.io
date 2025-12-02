/* FILE: index.html */
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
    <div class="container topbar">
      <div class="brand">
        <div>
          <h1>BBB Transport — Computational Modeling</h1>
          <div class="muted">Predictive simulation & educational tools for drug delivery across the blood–brain barrier</div>
        </div>
      </div>

      <nav class="mainnav">
        <a href="index.html" aria-current="page">Home</a>
        <a href="about.html">Research Plan</a>
        <a href="methods.html">Methods & Results</a>
        <a href="simulate.html">Simulator</a>
        <a href="poster.html">Poster & Files</a>
        <a href="contact.html">Contact</a>
      </nav>
    </div>
  </header>

  <main class="container hero">
    <section class="intro card">
      <h2>Bridging molecular design and transport behavior</h2>
      <p class="lead">We develop a predictive computational framework to model, simulate, and optimize transport across the blood–brain barrier (BBB). Our stack combines mechanistic ODEs, stochastic particle simulations, and machine learning-driven analysis to accelerate rational design of therapeutic vectors that reach the CNS.</p>

      <div class="cta-row">
        <a class="btn" href="simulate.html">Try the Enhanced Simulator</a>
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
        <div class="kpi"><strong>1M+</strong><span>Simulated particles (total)</span></div>
        <div class="kpi"><strong>Open-source</strong><span>Planned release</span></div>
      </div>
    </section>
  </main>

  <footer class="footer">
    <div class="container">
      <small>Poster: <code>Quant2 Final Poster.pdf</code> — Notebook: <code>Final Project (1).ipynb</code></small>
      <p>© 2025 Alex — Computational Modeling of BBB transport</p>
    </div>
  </footer>
</body>
</html>

--------------------------------------------------------------------------------
/* FILE: styles.css */
:root{
  --bg:#f6f7fb; --card:#ffffff; --accent:#0b5fff; --muted:#263238; --glass: rgba(255,255,255,0.7);
  --radius:12px;
}
*{box-sizing:border-box}
body{font-family:Inter,system-ui,Segoe UI,Roboto,Arial,sans-serif;margin:0;background:var(--bg);color:var(--muted);-webkit-font-smoothing:antialiased}
.container{max-width:1100px;margin:0 auto;padding:20px}
.topbar{display:flex;align-items:center;justify-content:space-between;gap:20px}
.brand h1{margin:0;color:#062a7c;font-size:20px}
.muted{color:#6b7280;font-size:13px}
.mainnav a{margin-left:16px;color:var(--accent);text-decoration:none;font-weight:600}
.navwrap{background:linear-gradient(90deg,#0b5fff15,#0b5fff06);padding:18px;border-bottom:1px solid #e6ecff}
.hero{padding:36px 20px}
.lead{font-size:16px;color:#1f2937}
.grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:18px;margin-top:18px}
.card{background:var(--card);padding:18px;border-radius:var(--radius);box-shadow:0 8px 24px rgba(12,18,45,0.06)}
.highlight{margin-top:18px}
.kpis{display:flex;gap:12px;flex-wrap:wrap}
.kpi{background:linear-gradient(180deg,#fbfdff,#f7fbff);padding:10px;border-radius:10px;min-width:120px;text-align:center}
.btn{display:inline-block;padding:10px 14px;border-radius:10px;background:var(--accent);color:white;text-decoration:none;font-weight:700;margin-right:8px}
.btn.ghost{background:transparent;color:var(--accent);border:2px solid var(--accent)}
.footer{padding:24px 20px;text-align:center;color:#889;margin-top:36px}
.grid-2{display:grid;grid-template-columns:1fr 320px;gap:18px}
.small{font-size:13px;color:#6b7280}
/* Simulation page tweaks */
.sim-canvas{width:100%;height:460px;border-radius:10px;display:block;background:linear-gradient(180deg,#ffffff,#f3f6ff)}
.controls .control{margin-bottom:12px}
label{display:block;margin-bottom:6px;font-weight:600;color:#223}
input[type=range]{width:100%}
.select, select{width:100%;padding:8px;border-radius:8px;border:1px solid #e6edf8;background:#fff}
.row{display:flex;gap:10px;align-items:center}
.metric{background:#fff;padding:10px;border-radius:10px;box-shadow:0 6px 14px rgba(10,15,40,0.04)}
.footer small code{background:#fff;padding:4px;border-radius:6px}
@media (max-width:920px){
  .grid-3{grid-template-columns:1fr}
  .grid-2{grid-template-columns:1fr}
  .topbar{flex-direction:column;align-items:flex-start}
  .mainnav{margin-top:10px}
}

--------------------------------------------------------------------------------
/* FILE: about.html */
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
    <div class="container topbar">
      <div class="brand">
        <h1>Research Plan — BBB Transport</h1>
        <div class="muted">Graduate Research Plan Statement</div>
      </div>

      <nav class="mainnav">
        <a href="index.html">Home</a>
        <a href="about.html" aria-current="page">Research Plan</a>
        <a href="methods.html">Methods</a>
        <a href="simulate.html">Simulator</a>
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

--------------------------------------------------------------------------------
/* FILE: methods.html */
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
    <div class="container topbar">
      <div class="brand"><h1>Methods & Results</h1></div>
      <nav class="mainnav">
        <a href="index.html">Home</a>
        <a href="about.html">Research Plan</a>
        <a href="methods.html" aria-current="page">Methods</a>
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
        <li>Smaller particles (&lt;80 nm) with neutral-to-moderate positive charge and amphiphilic patches showed improved crossing probabilities in simulations.</li>
        <li>Simulated trends aligned with literature: receptor-mediated strategies outperform passive diffusion for large biologics.</li>
        <li>ML feature importance highlighted size, charge distribution, and hydrophobic surface fraction as top predictors.</li>
      </ul>

      <h3>Data sources</h3>
      <p>We integrate published experimental kinetics, imaging-derived permeability datasets, and internal simulations. The final site will link to our code repository and datasets for reproducible research.</p>
    </section>
  </main>

  <footer class="footer"><div class="container">© 2025 Alex — Methods</div></footer>
</body>
</html>

--------------------------------------------------------------------------------
/* FILE: poster.html */
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Poster & Project Files</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="navwrap">
    <div class="container topbar">
      <div class="brand"><h1>Poster & Files</h1></div>
      <nav class="mainnav">
        <a href="index.html">Home</a>
        <a href="simulate.html">Simulator</a>
        <a href="poster.html" aria-current="page">Poster</a>
      </nav>
    </div>
  </header>

  <main class="container">
    <section class="card">
      <h2>Final Project Poster</h2>
      <p>Click to open or download the poster. Upload <code>Quant2 Final Poster.pdf</code> to the repository root for GitHub Pages. Similarly, upload <code>Final Project (1).ipynb</code> for direct download.</p>
      <p><a class="btn" href="Quant2%20Final%20Poster.pdf" target="_blank" rel="noopener">Open Poster PDF</a></p>

      <div style="margin-top:18px">
        <h3>Final Project Notebook</h3>
        <p><a class="btn ghost" href="Final%20Project%20(1).ipynb" target="_blank" rel="noopener">Download Notebook</a></p>
      </div>
    </section>
  </main>

  <footer class="footer"><div class="container">© 2025 Alex — Poster</div></footer>
</body>
</html>

--------------------------------------------------------------------------------
/* FILE: contact.html */
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Contact — BBB Transport</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="navwrap">
    <div class="container topbar">
      <div class="brand"><h1>Contact</h1></div>
      <nav class="mainnav">
        <a href="index.html">Home</a>
        <a href="poster.html">Poster</a>
        <a href="contact.html" aria-current="page">Contact</a>
      </nav>
    </div>
  </header>

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

--------------------------------------------------------------------------------
/* FILE: simulate.html */
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Interactive BBB Simulator — Upgraded</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="navwrap">
    <div class="container topbar">
      <div class="brand"><h1>Interactive Simulator</h1><div class="muted">High-performance diffusion + receptor demo</div></div>
      <nav class="mainnav"><a href="index.html">Home</a><a href="simulate.html" aria-current="page">Simulator</a><a href="methods.html">Methods</a></nav>
    </div>
  </header>

  <main class="container">
    <section class="card">
      <h2>Particle diffusion & barrier crossing — Enhanced</h2>
      <p class="small">This upgraded demo visualizes Brownian-like particle motion in a 2D domain with a vertical "BBB" barrier. New features: receptor binding simulation (receptor density slider), deterministic RNG seed for reproducibility, better performance (particle pooling), timeline chart of crossing fraction, and CSV export.</p>

      <div class="grid-2" style="margin-top:16px">
        <div>
          <canvas id="simCanvas" class="sim-canvas" width="900" height="460"></canvas>

          <div style="display:flex;gap:10px;margin-top:12px;flex-wrap:wrap">
            <button id="startBtn" class="btn">Start</button>
            <button id="pauseBtn" class="btn ghost">Pause</button>
            <button id="resetBtn" class="btn ghost">Reset</button>
            <button id="exportBtn" class="btn" title="Export crossing timeline as CSV">Export CSV</button>
            <div class="metric" style="margin-left:auto"><strong>Crossed:</strong> <span id="crossed">0</span> / <span id="total">0</span></div>
          </div>

          <div style="margin-top:12px" class="card">
            <h3 style="margin-top:0">Crossing fraction timeline</h3>
            <canvas id="chartCanvas" width="900" height="140" style="width:100%;height:140px;border-radius:8px;background:#fff"></canvas>
            <div class="small" style="margin-top:6px">The chart shows the moving estimate of crossing fraction over time.</div>
          </div>
        </div>

        <aside class="card controls">
          <div class="control">
            <label>Particle count: <span id="pcountLabel">1000</span></label>
            <input id="pcount" type="range" min="100" max="5000" value="1000" />
          </div>

          <div class="control">
            <label>Particle radius (nm): <span id="radiusLabel">50</span></label>
            <input id="radius" type="range" min="5" max="200" value="50" />
            <div class="small">(Smaller particles generally diffuse faster.)</div>
          </div>

          <div class="control">
            <label>Diffusion coefficient D (μm²/s): <span id="dLabel">4.0</span></label>
            <input id="D" type="range" min="0.2" max="20" step="0.1" value="4.0" />
          </div>

          <div class="control">
            <label>Barrier permeability (0–1): <span id="permLabel">0.06</span></label>
            <input id="perm" type="range" min="0" max="1" step="0.01" value="0.06" />
            <div class="small">Higher = easier crossing when particles encounter pores/receptors.</div>
          </div>

          <div class="control">
            <label>Receptor density (0–1): <span id="receptorLabel">0.12</span></label>
            <input id="receptor" type="range" min="0" max="1" step="0.01" value="0.12" />
            <div class="small">Higher receptor density increases chance of receptor-mediated transcytosis.</div>
          </div>

          <div class="control">
            <label>Charge bias</label>
            <select id="charge">
              <option value="neutral">Neutral</option>
              <option value="positive">Slightly positive (attracts to barrier)</option>
              <option value="negative">Slightly negative (repelled)</option>
            </select>
          </div>

          <div class="control">
            <label>Deterministic RNG seed (empty = random)</label>
            <input id="seed" type="text" placeholder="e.g., 42" />
            <div class="small">Set a seed for reproducible runs (integers only).</div>
          </div>

          <div class="control">
            <div class="small">Tip: try increasing receptor density and permeability to see many crossing events. Use the seed to compare two parameter sets reproducibly.</div>
          </div>
        </aside>
      </div>
    </section>
  </main>

  <footer class="footer"><div class="container">© 2025 Alex — Interactive Simulator</div></footer>

  <script>
  /**************************************************************************
   * Upgraded simulator JS - fully client-side
   *
   * Responsibilities:
   *  - Efficient particle rendering (pooling + batched drawing)
   *  - Receptor-mediated crossing probability + passive crossing
   *  - Deterministic RNG seed support (Mulberry32)
   *  - Timeline chart (canvas)
   *  - CSV export of timeline
   **************************************************************************/

  (function(){
    // --- Utilities
    function mulberry32(a) {
      return function() {
        var t = a += 0x6D2B79F5;
        t = Math.imul(t ^ t >>> 15, t | 1);
        t ^= t + Math.imul(t ^ t >>> 7, t | 61);
        return ((t ^ t >>> 14) >>> 0) / 4294967296;
      }
    }
    function randFactory(seed){
      if(seed == null || seed === '') return Math.random;
      const s = Number(seed) | 0;
      if(Number.isNaN(s)) return Math.random;
      return mulberry32(s);
    }
    function downloadText(filename, text){
      const blob = new Blob([text], {type: 'text/csv'});
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url;
      a.download = filename;
      a.click();
      URL.revokeObjectURL(url);
    }

    // --- DOM elements & controls
    const canvas = document.getElementById('simCanvas');
    const ctx = canvas.getContext('2d');
    const chartCanvas = document.getElementById('chartCanvas');
    const chartCtx = chartCanvas.getContext('2d');

    const startBtn = document.getElementById('startBtn');
    const pauseBtn = document.getElementById('pauseBtn');
    const resetBtn = document.getElementById('resetBtn');
    const exportBtn = document.getElementById('exportBtn');

    const pcount = document.getElementById('pcount');
    const pcountLabel = document.getElementById('pcountLabel');
    const radius = document.getElementById('radius');
    const radiusLabel = document.getElementById('radiusLabel');
    const Dslider = document.getElementById('D');
    const dLabel = document.getElementById('dLabel');
    const perm = document.getElementById('perm');
    const permLabel = document.getElementById('permLabel');
    const receptor = document.getElementById('receptor');
    const receptorLabel = document.getElementById('receptorLabel');
    const charge = document.getElementById('charge');
    const crossedEl = document.getElementById('crossed');
    const totalEl = document.getElementById('total');
    const seedInput = document.getElementById('seed');

    // update label displays
    function wireLabels(){
      pcountLabel.textContent = pcount.value;
      radiusLabel.textContent = radius.value;
      dLabel.textContent = Dslider.value;
      permLabel.textContent = perm.value;
      receptorLabel.textContent = receptor.value;
    }
    [pcount, radius, Dslider, perm, receptor].forEach(el => el.addEventListener('input', wireLabels));
    wireLabels();

    // responsive canvas sizing
    function fitCanvas() {
      const rect = canvas.getBoundingClientRect();
      const DPR = window.devicePixelRatio || 1;
      canvas.width = Math.floor(rect.width * DPR);
      canvas.height = Math.floor(rect.height * DPR);
      ctx.setTransform(DPR, 0, 0, DPR, 0, 0);

      const crect = chartCanvas.getBoundingClientRect();
      chartCanvas.width = Math.floor(crect.width * DPR);
      chartCanvas.height = Math.floor(crect.height * DPR);
      chartCtx.setTransform(DPR,0,0,DPR,0,0);
      drawBackground();
      drawChart();
    }
    window.addEventListener('resize', fitCanvas);
    fitCanvas();

    // simulation state
    let rng = Math.random;
    let particles = [];
    let totalLaunched = 0;
    let crossed = 0;
    let running = false;
    let lastTime = null;
    let accumulatedTime = 0;

    // timeline data (sampled every sampleInterval seconds)
    const timeline = [];
    const sampleInterval = 0.5; // seconds

    // Particle pool factory
    function createParticle(x,y,radiusPx){
      return {
        x, y,
        vx: 0, vy: 0,
        radiusPx,
        crossed: false,
        alive: true
      };
    }

    function initParticles(){
      particles = [];
      crossed = 0;
      totalLaunched = Number(pcount.value) | 0;
      const startXMin = 8;
      const startXMax = (canvas.clientWidth/ (window.devicePixelRatio||1))/2 - 20;
      const height = (canvas.clientHeight/ (window.devicePixelRatio||1));
      const rpx = Math.max(2, (Number(radius.value)/20));
      for(let i=0;i<totalLaunched;i++){
        const x = startXMin + (rng() * Math.max(1, startXMax - startXMin));
        const y = 8 + rng()*(height - 16);
        particles.push(createParticle(x,y,rpx));
      }
      crossedEl.textContent = crossed;
      totalEl.textContent = totalLaunched;
      timeline.length = 0;
      pushTimelinePoint(0, 0);
    }

    // Draw background (regions + barrier)
    function drawBackground(){
      // clear with slight gradient
      const w = canvas.clientWidth / (window.devicePixelRatio||1);
      const h = canvas.clientHeight / (window.devicePixelRatio||1);
      ctx.clearRect(0,0,w,h);
      // left region
      const grad = ctx.createLinearGradient(0,0,0,h);
      grad.addColorStop(0, '#ffffff');
      grad.addColorStop(1, '#f3f6ff');
      ctx.fillStyle = grad;
      ctx.fillRect(0,0,w,h);

      // barrier
      const bx = w/2;
      ctx.fillStyle = '#062a7c';
      ctx.fillRect(bx-4, 0, 8, h);

      // pores (visual)
      ctx.save();
      ctx.globalAlpha = 0.06;
      for(let i=0;i<12;i++){
        const py = (i+0.5)*h/12;
        ctx.beginPath();
        ctx.arc(bx, py, 16, 0, Math.PI*2);
        ctx.fillStyle = '#fff';
        ctx.fill();
      }
      ctx.restore();

      // labels
      ctx.fillStyle = '#223';
      ctx.font = '13px system-ui, Arial';
      ctx.fillText('Bloodstream (inlet)', 12, 18);
      ctx.fillText('Brain (target)', w - 120, 18);
    }

    // Physics step: Brownian with optional drift/charge bias; barrier interaction rules
    function stepSimulation(dt){
      const D = Number(Dslider.value); // μm^2 / s (visual mapping)
      const scale = 0.7; // visual scale factor
      const sigma = Math.sqrt(2 * D * dt) * scale; // displacement magnitude
      const permVal = Number(perm.value);
      const receptorDensity = Number(receptor.value);
      const chargeBias = charge.value;

      const w = canvas.clientWidth/(window.devicePixelRatio||1);
      const h = canvas.clientHeight/(window.devicePixelRatio||1);
      const bx = w/2;

      for(const p of particles){
        if(!p.alive) continue;
        // Brownian-like displacement
        p.x += (rng()*2 - 1) * sigma * 10;
        p.y += (rng()*2 - 1) * sigma * 10;

        // boundary reflect
        if(p.y < p.radiusPx + 2) p.y = p.radiusPx + 2;
        if(p.y > h - (p.radiusPx + 2)) p.y = h - (p.radiusPx + 2);

        // charge bias: tiny horizontal drift
        if(chargeBias === 'positive') p.x += 0.018 * sigma * 8;
        else if(chargeBias === 'negative') p.x -= 0.018 * sigma * 8;

        // barrier interaction
        if(!p.crossed && p.x + p.radiusPx >= bx - 4){
          // receptor-mediated crossing chance
          const sizeFactor = Math.max(0.01, 1 - (Number(radius.value) / 260)); // bigger -> smaller factor
          const receptorEffect = 1 + receptorDensity * 2.5; // amplifies crossing by receptors
          const baseProb = permVal * sizeFactor * receptorEffect;

          // Additional boost for positive charge (illustrative)
          let prob = baseProb;
          if(chargeBias === 'positive') prob *= 1.5;
          // Cap prob moderately
          prob = Math.min(0.95, prob);

          // stochastic outcome
          if(rng() < prob){
            // crosses
            p.crossed = true;
            // move to right side (randomly distributed)
            p.x = bx + 6 + rng()* (w - bx - 20);
            crossed++;
            // leave alive so visible after crossing
          } else {
            // reflect
            p.x = bx - (p.radiusPx + 8) - rng()*4;
          }
        }

        // keep inside canvas
        if(p.x < 4) p.x = 4;
        if(p.x > w - 4) p.x = w - 4;
      }
    }

    // render particles (batched)
    function renderParticles(){
      const w = canvas.clientWidth/(window.devicePixelRatio||1);
      const h = canvas.clientHeight/(window.devicePixelRatio||1);
      drawBackground();

      // draw left region tint and right region tint subtle
      // draw particles: cross = blue, not cross = teal
      ctx.save();
      for(const p of particles){
        ctx.beginPath();
        ctx.fillStyle = p.crossed ? 'rgba(11,95,255,0.95)' : 'rgba(10,130,150,0.85)';
        ctx.arc(p.x, p.y, p.radiusPx, 0, Math.PI*2);
        ctx.fill();
      }
      ctx.restore();
    }

    // timeline sampling
    let sampleTimer = 0;
    function pushTimelinePoint(timeSec, fraction){
      timeline.push({t: timeSec, fraction});
      // keep window length manageable (e.g., last 600 points)
      if(timeline.length > 2000) timeline.shift();
    }

    // chart draw (simple line chart)
    function drawChart(){
      const w = chartCanvas.clientWidth/(window.devicePixelRatio||1);
      const h = chartCanvas.clientHeight/(window.devicePixelRatio||1);
      chartCtx.clearRect(0,0,w,h);

      // background
      chartCtx.fillStyle = '#fbfdff';
      chartCtx.fillRect(0,0,w,h);

      // axes
      chartCtx.strokeStyle = '#e6eefc';
      chartCtx.lineWidth = 1;
      chartCtx.beginPath();
      chartCtx.moveTo(0,h-1);
      chartCtx.lineTo(w,h-1);
      chartCtx.stroke();

      if(timeline.length < 2) return;
      // compute min/max t
      const t0 = timeline[0].t;
      const tN = timeline[timeline.length-1].t;
      const tSpan = Math.max(1e-6, tN - t0);
      chartCtx.beginPath();
      for(let i=0;i<timeline.length;i++){
        const x = ((timeline[i].t - t0)/tSpan) * (w - 8) + 4;
        const y = h - (timeline[i].fraction) * (h - 12) - 6;
        if(i === 0) chartCtx.moveTo(x,y);
        else chartCtx.lineTo(x,y);
      }
      chartCtx.strokeStyle = '#0b5fff';
      chartCtx.lineWidth = 2;
      chartCtx.stroke();

      // last point marker
      const last = timeline[timeline.length-1];
      const lastX = ((last.t - t0)/tSpan) * (w - 8) + 4;
      const lastY = h - (last.fraction)*(h - 12) - 6;
      chartCtx.fillStyle = '#0b5fff';
      chartCtx.beginPath();
      chartCtx.arc(lastX, lastY, 3, 0, Math.PI*2);
      chartCtx.fill();
    }

    // main loop
    function loop(now){
      if(!running) return;
      if(lastTime == null) lastTime = now;
      const dtMs = Math.min(40, now - lastTime); // cap dt for stability
      const dt = dtMs / 1000; // seconds
      lastTime = now;

      stepSimulation(dt);
      renderParticles();

      accumulatedTime += dt;
      sampleTimer += dt;
      if(sampleTimer >= sampleInterval){
        const fraction = totalLaunched > 0 ? (crossed / totalLaunched) : 0;
        pushTimelinePoint(accumulatedTime, fraction);
        sampleTimer = 0;
        drawChart();
      }
      // update UI numbers
      crossedEl.textContent = crossed;
      requestAnimationFrame(loop);
    }

    // controls handlers
    startBtn.addEventListener('click', ()=>{
      // set RNG
      rng = randFactory(seedInput.value);
      if(!running){
        // start
        running = true;
        lastTime = null;
        if(particles.length === 0) initParticles();
        requestAnimationFrame(loop);
        startBtn.textContent = 'Running...';
        startBtn.disabled = true;
        pauseBtn.disabled = false;
      }
    });

    pauseBtn.addEventListener('click', ()=>{
      if(running){
        running = false;
        startBtn.textContent = 'Start';
        startBtn.disabled = false;
        pauseBtn.textContent = 'Resume';
      } else {
        running = true;
        pauseBtn.textContent = 'Pause';
        lastTime = null;
        requestAnimationFrame(loop);
      }
    });

    resetBtn.addEventListener('click', ()=>{
      running = false;
      startBtn.textContent = 'Start';
      startBtn.disabled = false;
      pauseBtn.textContent = 'Pause';
      crossed = 0;
      initParticles();
      drawBackground();
      renderParticles();
      drawChart();
    });

    exportBtn.addEventListener('click', ()=>{
      // prepare CSV: time, fraction
      let csv = 'time_s, crossed_fraction\\n';
      for(const pt of timeline){
        csv += `${pt.t.toFixed(3)},${pt.fraction}\\n`;
      }
      downloadText('crossing_timeline.csv', csv);
    });

    // init
    initParticles();
    drawBackground();
    renderParticles();
    drawChart();

    // ensure labels show correct initial numbers
    pcount.addEventListener('input', ()=>{
      pcountLabel.textContent = pcount.value;
    });

  })();
  </script>
</body>
</html>
