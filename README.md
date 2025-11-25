<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Computational Modeling of Drug Transport Across the BBB</title>
  <style>
    :root{
      --bg:#f6f7fb;--card:#ffffff;--accent:#0b5fff;--muted:#556;--maxw:1100px;
      --glass: rgba(255,255,255,0.6);
    }
    *{box-sizing:border-box}
    body{margin:0;font-family:Inter,system-ui,Arial,Helvetica,sans-serif;background:var(--bg);color:var(--muted);-webkit-font-smoothing:antialiased}
    header{background:linear-gradient(90deg,#0b5fff22,#0b5fff11);padding:28px 20px;border-bottom:1px solid #e6ecff}
    .wrap{max-width:var(--maxw);margin:0 auto}
    .brand{display:flex;gap:16px;align-items:center}
    .brand h1{margin:0;font-size:20px;color:#062a7c}
    nav{margin-top:12px}
    nav a{margin-right:14px;color:var(--accent);text-decoration:none;font-weight:600}
    .hero{padding:48px 20px;background:transparent;text-align:left}
    .lead{font-size:18px;color:#223}
    .grid{display:grid;grid-template-columns:1fr 340px;gap:24px;margin-top:28px}
    .card{background:var(--card);padding:18px;border-radius:12px;box-shadow:0 6px 18px rgba(15,23,42,0.06)}
    h2{margin-top:0;color:#062a7c}
    ul{padding-left:1.1rem}
    footer{padding:24px 20px;text-align:center;color:#889}
    .kpi{display:flex;gap:12px;flex-wrap:wrap;margin-top:12px}
    .kpi .metric{background:linear-gradient(180deg,#fbfdff,#f7fbff);padding:12px;border-radius:10px;min-width:110px}
    .muted{color:#6b7280}
    .btn{display:inline-block;padding:10px 14px;border-radius:8px;background:var(--accent);color:#fff;text-decoration:none;font-weight:600}
    .pdfframe{width:100%;height:600px;border:0;border-radius:8px}
    @media (max-width:900px){.grid{grid-template-columns:1fr}.pdfframe{height:400px}}
  </style>
</head>
<body>
  <header>
    <div class="wrap">
      <div class="brand">
        <div>
          <h1>Computational Modeling of Drug Transport Across the Blood–Brain Barrier</h1>
          <div class="muted">A project by Alex — Computational & Biomaterials Modeling</div>
        </div>
      </div>
      <nav>
        <a href="#about">About</a>
        <a href="#methods">Methods</a>
        <a href="#results">Results</a>
        <a href="#poster">Poster (PDF)</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <main class="wrap">
    <section class="hero">
      <p class="lead">We model transport across the blood–brain barrier (BBB) using differential equations, stochastic diffusion simulations, and machine learning-driven molecular feature analysis to predict which nanoparticle and molecular features enhance permeability.</p>
    </section>

    <section class="grid">
      <div>
        <div class="card" id="about">
          <h2>Introduction</h2>
          <p>The blood–brain barrier prevents &gt;98% of therapeutics from reaching the central nervous system. Effective delivery to the brain remains a major challenge in neuroscience and pharmacology. Our computational framework aims to clarify transport mechanisms and accelerate rational design of delivery systems.</p>

          <h3>Objectives</h3>
          <ul>
            <li>Develop a computational framework to simulate BBB transport (kinetic & stochastic models).</li>
            <li>Quantify diffusion of nanoparticles and biologically derived molecules with varying size, charge, and surface chemistry.</li>
            <li>Integrate experimental datasets and stochastic modeling for predictive insights.</li>
          </ul>

          <h3 id="methods">Methods</h3>
          <ul>
            <li><strong>Deterministic models:</strong> Differential equations describing transcytosis, diffusion, and clearance.</li>
            <li><strong>Stochastic simulations:</strong> Brownian and subdiffusive particle models to capture heterogeneity in transport.</li>
            <li><strong>Molecular feature analysis:</strong> Machine learning to identify features associated with higher BBB permeability.</li>
          </ul>

          <h3 id="results">Summary & Results</h3>
          <p>We combine modeling and ML to prioritize nanoparticle design features (size range, surface charge, hydrophobic patches) that correlate with increased transport across BBB-like interfaces. Our simulations reproduce expected trends from experimental literature and generate hypotheses that will be validated experimentally.</p>

          <h3>Applications</h3>
          <ul>
            <li>Accelerate CNS drug development by guiding nanoparticle and small-molecule design.</li>
            <li>Provide an open-source simulation platform for education and research.</li>
            <li>Predict targeted delivery strategies relevant to neurodegenerative diseases and synthetic biology.</li>
          </ul>
        </div>

        <div class="card" style="margin-top:18px;">
          <h2>Current Projects</h2>
          <ul>
            <li>Stimuli-responsive polymer brushes for ophthalmic and CNS delivery.</li>
            <li>Open-source diffusion simulator with tunable boundary conditions.</li>
            <li>ML pipeline for feature selection and transport prediction.</li>
          </ul>

          <h2>Key Metrics</h2>
          <div class="kpi">
            <div class="metric"><div class="muted">Model runs</div><div><strong>120+</strong></div></div>
            <div class="metric"><div class="muted">Simulated particles</div><div><strong>1M+</strong></div></div>
            <div class="metric"><div class="muted">Top features</div><div><strong>Size, Charge, Hydrophobicity</strong></div></div>
          </div>
        </div>
      </div>

      <aside>
        <div class="card">
          <h2>Poster</h2>
          <p class="muted">View or download the poster that accompanies this site.</p>
          <!-- The href below points to the local poster file included with the project. -->
          <p><a class="btn" href="/mnt/data/Quant2 Final Poster.pdf" target="_blank">Open Poster PDF</a></p>
          <p class="muted">If you host this site on GitHub Pages, put <code>Quant2 Final Poster.pdf</code> in the repository root so the link works as <code>/Quant2 Final Poster.pdf</code>.</p>
        </div>

        <div class="card" style="margin-top:18px;">
          <h3>Contact</h3>
          <p>Alex — <a href="mailto:alex@example.edu">alex@example.edu</a></p>
          <p class="muted">Interested in collaboration or code? The simulation platform will be released as open-source.</p>
        </div>
      </aside>
    </section>

    <section class="card" style="margin:28px 0;">
      <h2>Embedded Poster Preview</h2>
      <!-- Embedded viewer that uses the uploaded poster file path. -->
      <iframe class="pdfframe" src="/mnt/data/Quant2 Final Poster.pdf"></iframe>
      <p class="muted" style="margin-top:12px">(If the embedded preview fails in your browser, click <a href="/mnt/data/Quant2 Final Poster.pdf" target="_blank">here</a> to download the PDF.)</p>
      <p class="muted">Source document: Quant2 Final Poster. fileciteturn1file0</p>
    </section>

  </main>

  <footer>
    <div class="wrap">© 2025 Alex — Computational Modeling of BBB transport</div>
  </footer>
</body>
</html>
