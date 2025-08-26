<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Akmal — Portfolio</title>
  <meta name="description" content="From Aerospace Engineering to Business — projects, case studies, and the journey." />
  <meta property="og:title" content="Akmal — Portfolio" />
  <meta property="og:description" content="From Aerospace Engineering to Business — projects, case studies, and the journey." />
  <meta property="og:type" content="website" />
  <meta name="theme-color" content="#0f172a" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg: #0b1020;
      --panel:#0f172a;
      --muted:#94a3b8;
      --text:#e2e8f0;
      --accent:#60a5fa;
      --card:#11172b;
      --ring:#1d4ed8;
    }
    @media (prefers-color-scheme: light) {
      :root{
        --bg:#f8fafc;--panel:#ffffff;--muted:#475569;--text:#0f172a;--accent:#2563eb;--card:#ffffff;--ring:#3b82f6;
      }
      body{background-image: radial-gradient(600px 200px at 20% -10%, #e0e7ff40, transparent), radial-gradient(600px 200px at 120% -10%, #bae6fd40, transparent);}  
    }
    *{box-sizing:border-box}
    html,body{margin:0}
    body{font-family:Inter,system-ui,Arial,Helvetica,sans-serif;background:var(--bg);color:var(--text);line-height:1.6}
    .container{max-width:1000px;margin-inline:auto;padding:24px}
    header{position:sticky;top:0;backdrop-filter:saturate(140%) blur(6px);background:color-mix(in oklab, var(--bg) 80%, transparent);border-bottom:1px solid #ffffff14;z-index:50}
    nav{display:flex;gap:16px;align-items:center;justify-content:space-between}
    nav a{color:var(--text);text-decoration:none;font-weight:600;opacity:.9}
    nav a:hover{opacity:1}
    .btn{display:inline-flex;align-items:center;gap:10px;background:var(--accent);color:white;padding:10px 14px;border-radius:14px;text-decoration:none;font-weight:700;box-shadow:0 8px 24px #60a5fa3a;border:1px solid #ffffff22}
    .btn.secondary{background:transparent;color:var(--text);border:1px solid #ffffff22}
    .hero{padding:64px 0 32px;display:grid;grid-template-columns:1.2fr .8fr;gap:28px;align-items:center}
    .hero h1{line-height:1.1;font-size:clamp(28px, 4.2vw, 48px);margin:8px 0}
    .hero p{color:var(--muted)}
    .tag{display:inline-block;border:1px solid #ffffff2a;padding:6px 10px;border-radius:999px;font-size:12px;letter-spacing:.3px;color:var(--muted)}
    .card{background:var(--card);border:1px solid #ffffff14;border-radius:20px;padding:18px}
    .grid{display:grid;gap:18px}
    .grid.cols-3{grid-template-columns:repeat(3, 1fr)}
    .grid.cols-2{grid-template-columns:repeat(2, 1fr)}
    @media (max-width:880px){
      .hero{grid-template-columns:1fr}
      .grid.cols-3{grid-template-columns:1fr}
      .grid.cols-2{grid-template-columns:1fr}
    }
    .section{margin:26px 0}
    h2{font-size:clamp(20px, 2.8vw, 28px);margin:0 0 12px}
    h3{margin:0 0 6px}
    .muted{color:var(--muted)}
    .avatar{width:100%;aspect-ratio:1/1;object-fit:cover;border-radius:22px;border:1px solid #ffffff1a}
    .kpis{display:flex;gap:14px;flex-wrap:wrap}
    .kpi{flex:1;min-width:150px;background:var(--card);padding:14px;border-radius:14px;border:1px solid #ffffff12}
    .kpi strong{font-size:20px}
    .project{display:flex;flex-direction:column;gap:8px}
    .pill{display:inline-block; padding:4px 10px;border-radius:999px;background:#ffffff10;border:1px solid #ffffff25;font-size:12px}
    .timeline{position:relative;margin-left:8px}
    .timeline::before{content:"";position:absolute;left:10px;top:0;bottom:0;width:2px;background:#ffffff1f}
    .t-item{position:relative;padding-left:32px;margin:16px 0}
    .t-item::before{content:"";position:absolute;left:4px;top:6px;width:14px;height:14px;border-radius:999px;background:var(--accent);box-shadow:0 0 0 3px #60a5fa33}
    footer{padding:36px 0;color:var(--muted)}
    .sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border-width:0}
    .link{color:var(--accent);text-decoration:none}
    .flex{display:flex;gap:10px;align-items:center;flex-wrap:wrap}
    .download{display:inline-flex;align-items:center;gap:10px;padding:10px 14px;border-radius:12px;border:1px dashed #ffffff33;color:var(--text);text-decoration:none}
    .project-img{width:100%;aspect-ratio:16/9;object-fit:cover;border-radius:14px;border:1px solid #ffffff12;background:#ffffff08}
    /* Simple focus ring */
    :focus-visible{outline:3px solid var(--ring);outline-offset:3px;border-radius:6px}
  </style>
</head>
<body>
  <header>
    <div class="container">
      <nav>
        <a href="#home" aria-label="Home">Akmal</a>
        <div class="flex" aria-label="Primary Navigation">
          <a href="#projects">Projects</a>
          <a href="#skills">Skills</a>
          <a href="#journey">Journey</a>
          <a href="#contact">Contact</a>
          <a class="btn secondary" href="#cv">Download CV</a>
        </div>
      </nav>
    </div>
  </header>

  <main id="home" class="container">
    <section class="hero">
      <div>
        <span class="tag">From Aerospace → Business</span>
        <h1>Hi, I’m Akmal. I build, analyze, and grow business ideas.</h1>
        <p class="muted">Originally trained in Aerospace Engineering, I discovered my drive is in entrepreneurship and management. Here I document my projects, experiments, and the journey that led me to pursue a business degree overseas.</p>
        <div class="kpis" style="margin-top:14px">
          <div class="kpi"><strong id="kpi-sales">$12,400</strong><div class="muted">Total Sales (side hustles)</div></div>
          <div class="kpi"><strong id="kpi-projects">7</strong><div class="muted">Projects Shipped</div></div>
          <div class="kpi"><strong id="kpi-courses">6</strong><div class="muted">Business Courses Completed</div></div>
        </div>
        <div class="flex" style="margin-top:18px">
          <a class="btn" href="#projects">See Projects</a>
          <a class="btn secondary" href="#about">About Me</a>
        </div>
      </div>
      <div>
        <img class="avatar" src="https://images.unsplash.com/photo-1527980965255-d3b416303d12?q=80&w=1000&auto=format&fit=crop" alt="Portrait placeholder"/>
      </div>
    </section>

    <section id="about" class="section">
      <div class="grid cols-2">
        <div class="card">
          <h2>About Me</h2>
          <p>I studied Aerospace Engineering at polytechnic in Singapore. Through side projects — reselling, small e‑commerce experiments, and helping friends promote services — I realized I love the <em>business</em> side: pricing, marketing, and turning data into decisions.</p>
          <p>Now, I’m pursuing a business degree overseas to combine technical rigor with management and entrepreneurship.</p>
          <div class="flex" style="margin-top:6px">
            <span class="pill">Analytical</span>
            <span class="pill">Builder-first</span>
            <span class="pill">Customer-obsessed</span>
          </div>
        </div>
        <div class="card">
          <h2>Highlights</h2>
          <ul>
            <li>📈 Grew a niche resell store to ~200 orders in 6 months</li>
            <li>🧭 Led ops for a small community event (120 attendees)</li>
            <li>🧮 Built Excel trackers for P&L and inventory</li>
            <li>🎯 Completed fundamentals in Marketing, Finance, and Excel</li>
          </ul>
        </div>
      </div>
    </section>

    <section id="projects" class="section">
      <h2>Projects & Case Studies</h2>
      <div class="grid cols-3">
        <article class="card project">
          <img class="project-img" src="https://images.unsplash.com/photo-1542744173-8e7e53415bb0?q=80&w=1200&auto=format&fit=crop" alt="Marketing dashboard placeholder" />
          <h3>Carousell Resale Store</h3>
          <p class="muted">Jan 2023 – Nov 2023</p>
          <p>Researched demand, sourced items, priced dynamically, and built a basic funnel. Documented P&L and conversion metrics.</p>
          <div class="flex">
            <span class="pill">Pricing</span>
            <span class="pill">Marketing</span>
            <span class="pill">P&L</span>
          </div>
          <a class="link" href="#" aria-label="View case study">View case study →</a>
        </article>
        <article class="card project">
          <img class="project-img" src="https://images.unsplash.com/photo-1556761175-4b46a572b786?q=80&w=1200&auto=format&fit=crop" alt="Operations planning placeholder" />
          <h3>Event Ops & Sponsorships</h3>
          <p class="muted">May 2023 – Jul 2023</p>
          <p>Coordinated logistics and small sponsors for a community event; created pitch deck and tracked ROI for partners.</p>
          <div class="flex">
            <span class="pill">Operations</span>
            <span class="pill">Partnerships</span>
            <span class="pill">Decks</span>
          </div>
          <a class="link" href="#" aria-label="View case study">View case study →</a>
        </article>
        <article class="card project">
          <img class="project-img" src="https://images.unsplash.com/photo-1543286386-2e659306cd6c?q=80&w=1200&auto=format&fit=crop" alt="Ecommerce mockup placeholder" />
          <h3>Shop Mock: Coffee Brand</h3>
          <p class="muted">Dec 2023</p>
          <p>Designed a mock D2C coffee brand with a landing page, CAC/LTV model, and a 3‑month content plan.</p>
          <div class="flex">
            <span class="pill">Branding</span>
            <span class="pill">Analytics</span>
            <span class="pill">Content</span>
          </div>
          <a class="link" href="#" aria-label="View case study">View case study →</a>
        </article>
      </div>
    </section>

    <section id="skills" class="section">
      <div class="grid cols-3">
        <div class="card">
          <h2>Skills</h2>
          <ul>
            <li>Marketing basics (funnels, CTAs, copy)</li>
            <li>Financial literacy (P&L, cashflow)</li>
            <li>Operations & logistics</li>
            <li>Excel/Sheets, Canva, basic HTML/CSS</li>
          </ul>
        </div>
        <div class="card">
          <h2>Courses</h2>
          <ul>
            <li>Google Digital Garage — Fundamentals of Digital Marketing</li>
            <li>Intro to Corporate Finance (Coursera)</li>
            <li>Excel for Business (LinkedIn Learning)</li>
          </ul>
        </div>
        <div class="card">
          <h2>Downloads</h2>
          <p id="cv" class="muted">Grab my latest resume and motivation letter.</p>
          <div class="flex">
            <a class="download" href="./Akmal_CV.pdf" download>⬇️ CV (PDF)</a>
            <a class="download" href="./Motivation_Letter.pdf" download>⬇️ Motivation (PDF)</a>
          </div>
        </div>
      </div>
    </section>

    <section id="journey" class="section">
      <div class="card">
        <h2>My Journey</h2>
        <div class="timeline" aria-label="Timeline of key moments">
          <div class="t-item"><strong>2021 — Aerospace Foundations</strong><div class="muted">Built analytical discipline and systems thinking.</div></div>
          <div class="t-item"><strong>2022 — First Side Hustles</strong><div class="muted">Resale experiments; learned pricing and customer service.</div></div>
          <div class="t-item"><strong>2023 — Community Event Ops</strong><div class="muted">Hands-on logistics, sponsors, and budgeting.</div></div>
          <div class="t-item"><strong>2024 — Decision to Pivot</strong><div class="muted">Committed to business degree overseas to scale my impact.</div></div>
        </div>
      </div>
    </section>

    <section id="contact" class="section">
      <div class="grid cols-2">
        <div class="card">
          <h2>Contact</h2>
          <p>Open to conversations, internships, and collaborations.</p>
          <p>📮 <a class="link" href="mailto:hello@example.com">hello@example.com</a></p>
          <p>🔗 <a class="link" href="https://www.linkedin.com" target="_blank" rel="noreferrer">LinkedIn</a> · <a class="link" href="https://github.com" target="_blank" rel="noreferrer">GitHub</a></p>
        </div>
        <div class="card">
          <h2>How this site works</h2>
          <p>This is a single, static HTML file — perfect for GitHub Pages. Edit the content below via the JSON block or directly in the HTML.</p>
          <details>
            <summary>Quick edit via JSON</summary>
            <pre id="dataPreview" style="white-space:pre-wrap;overflow:auto;max-height:220px;background:#00000020;padding:10px;border-radius:10px;border:1px solid #ffffff18"></pre>
          </details>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">
      <div class="flex" style="justify-content:space-between">
        <span>© <span id="year"></span> Akmal</span>
        <span class="muted">Built for admissions & internships</span>
      </div>
    </div>
  </footer>

  <!-- Simple data block so you can tweak numbers/content without hunting through markup -->
  <script id="portfolio-data" type="application/json">
  {
    "name": "Akmal",
    "email": "hello@example.com",
    "kpis": {"sales": "$12,400", "projects": 7, "courses": 6}
  }
  </script>
  <script>
    // Tiny helper to update KPIs and show JSON
    (function(){
      const year = new Date().getFullYear();
      document.getElementById('year').textContent = year;

      try {
        const dataEl = document.getElementById('portfolio-data');
        const data = JSON.parse(dataEl.textContent);
        if (data?.kpis) {
          document.getElementById('kpi-sales').textContent = data.kpis.sales;
          document.getElementById('kpi-projects').textContent = String(data.kpis.projects);
          document.getElementById('kpi-courses').textContent = String(data.kpis.courses);
        }
        const preview = document.getElementById('dataPreview');
        if (preview) preview.textContent = JSON.stringify(data, null, 2);
      } catch (e) {}
    })();
  </script>
</body>
</html>
