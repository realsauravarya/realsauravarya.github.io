<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Chiku — Portfolio</title>
  <meta name="description" content="Portfolio of Chiku — Web developer, system admin, and aspiring AI/tech creator." />

  <!-- Simple CSS reset + layout (single-file, no deps) -->
  <style>
    :root{
      --bg:#0f1724; --card:#111827; --muted:#94a3b8; --accent:#06b6d4; --glass: rgba(255,255,255,0.03);
      --maxw:1000px;
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:Inter,system-ui,Segoe UI,Roboto,'Helvetica Neue',Arial;color:#e6eef6;background:linear-gradient(180deg,var(--bg),#071028);}
    .wrap{max-width:var(--maxw);margin:36px auto;padding:24px}
    header{display:flex;align-items:center;justify-content:space-between;gap:16px}
    .brand{display:flex;align-items:center;gap:12px}
    .avatar{width:64px;height:64px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#7c3aed);display:flex;align-items:center;justify-content:center;color:#04192a;font-weight:700;font-size:20px}
    h1{margin:0;font-size:28px}
    p.lead{margin:6px 0 0;color:var(--muted)}

    main{margin-top:24px;display:grid;grid-template-columns:1fr 320px;gap:24px}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:18px;border-radius:12px;box-shadow:0 6px 18px rgba(2,6,23,0.6);border:1px solid rgba(255,255,255,0.03)}

    .hero{padding:18px}
    .meta{display:flex;flex-wrap:wrap;gap:8px;margin-top:12px}
    .tag{background:var(--glass);padding:6px 10px;border-radius:999px;font-size:13px;color:var(--muted)}

    .section{margin-top:16px}
    h2{margin:0 0 12px 0;font-size:16px}
    ul.skills{display:flex;flex-wrap:wrap;gap:8px;padding:0;margin:0;list-style:none}
    ul.skills li{padding:8px 10px;border-radius:8px;background:rgba(255,255,255,0.02);font-weight:600}

    .projects .project{margin-bottom:12px;padding:12px;border-radius:10px;background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.005));}
    .project h3{margin:0 0 6px 0}
    .project p{margin:0;color:var(--muted)}

    aside{position:relative}
    .contact-list{display:flex;flex-direction:column;gap:10px}
    .contact-list a{display:block;padding:10px;border-radius:8px;background:rgba(255,255,255,0.02);text-decoration:none;color:inherit}

    footer{margin-top:28px;color:var(--muted);text-align:center;font-size:13px}

    /* responsive */
    @media (max-width:900px){main{grid-template-columns:1fr} .avatar{width:56px;height:56px}}
  </style>
</head>
<body>
  <!--
    NOTE: This single-file portfolio is intended for GitHub Pages
    - Save as `index.html` in a repo, push to `main` (or gh-pages), then enable Pages
    - Editable areas are clearly marked with comments like <!-- EDIT: ... -->

    CHANGES/COMMENTS: Where to update (search for "EDIT:")
  -->

  <div class="wrap">
    <header>
      <div class="brand">
        <div class="avatar">C</div>
        <div>
          <h1>Chiku</h1>
          <p class="lead">Night‑shift cook &amp; freelance PHP / Systems dev — transitioning into AI &amp; infra.</p>
        </div>
      </div>

      <nav>
        <a href="#projects" style="color:var(--accent);text-decoration:none;font-weight:700">View projects →</a>
      </nav>
    </header>

    <main>
      <section class="card hero">
        <h2>About me</h2>
        <!-- EDIT: Update this paragraph with your short bio or keep as-is -->
        <p>I’m a developer with a BCA from Lovely Professional University and a Post‑Cert in Applied Network Infrastructure &amp; System Administration from Conestoga College (Jan 2024 — Apr 2025). I’ve worked as a web developer (PHP, API integrations) and run freelance IT projects, while managing ops and servers for small deployments. I’m focused on building tutorials, moving into AI/tech, and improving my French for Canadian PR.</p>

        <div class="meta">
          <!-- EDIT: Update tags as needed -->
          <span class="tag">BCA — Lovely Professional University (2016–2020)</span>
          <span class="tag">Conestoga — Network &amp; SysAdmin (2024–2025)</span>
          <span class="tag">Freelance PHP • APIs</span>
          <span class="tag">Linux • Proxmox • Hetzner</span>
        </div>

        <div class="section">
          <h2>Primary skills</h2>
          <ul class="skills">
            <!-- EDIT: Add or remove skills -->
            <li>PHP</li>
            <li>API Integrations</li>
            <li>Linux Systems</li>
            <li>Networking</li>
            <li>React / Frontend</li>
            <li>Python scripting</li>
            <li>Server ops / Proxmox</li>
          </ul>
        </div>

        <div class="section projects" id="projects">
          <h2>Selected projects</h2>

          <!-- EDIT: Replace the example projects below with your actual projects and links -->
          <div class="project">
            <h3>RawSetLabs (personal site)</h3>
            <p>Multiple VMs and subdomains for internal services — I manage hosting, DNS, and service configuration.</p>
          </div>

          <div class="project">
            <h3>RSS Reader + React UI</h3>
            <p>Frontend + Python backend for parsing RSS feeds, marking read/unread, and a tinder‑style feed viewer.</p>
          </div>

          <div class="project">
            <h3>API integrations (freelance)</h3>
            <p>Various PHP integrations with third‑party APIs — auth, scraping, and automation scripts.</p>
          </div>

        </div>

      </section>

      <aside class="card">
        <h2>Contact & links</h2>
        <div class="contact-list">
          <!-- EDIT: Replace the href values with your actual links -->
          <a href="https://github.com/your-username" target="_blank" rel="noopener">GitHub — your-username</a>
          <a href="https://www.linkedin.com/in/your-linkedin" target="_blank" rel="noopener">LinkedIn — your-linkedin</a>
          <a href="https://rawsetlabs.com" target="_blank" rel="noopener">RawSetLabs</a>
          <a href="mailto:you@example.com">Email — you@example.com</a>
        </div>

        <div class="section">
          <h2>Goals</h2>
          <ul style="margin:0;padding-left:18px;color:var(--muted)">
            <li>Transition into AI/tech role</li>
            <li>Grow YouTube tutorials &amp; LinkedIn presence</li>
            <li>Pay off student loan; stable freelance income</li>
            <li>Learn French for PR</li>
          </ul>
        </div>

        <div class="section">
          <h2>Quick CV</h2>
          <p style="margin:0;color:var(--muted)">BCA (2016–2020) · Web Dev at Logisquare (2016–2023) · Conestoga Cert (2024–2025)</p>
        </div>

      </aside>
    </main>

    <footer>
      <!-- EDIT: Change copyright or remove -->
      <div>© <span id="year"></span> Chiku — Built with HTML &amp; a little coffee.</div>
      <script>document.getElementById('year').textContent=new Date().getFullYear();</script>
    </footer>
  </div>
</body>
</html>
