<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>ACEN–UFS merSETA Risk Management Case Study • Jonathan Tager</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta name="description" content="Project management case study: ACEN–UFS merSETA circular economy capacity-building programme, including Agile/PMI-aligned risk register and dashboards." />
  <style>
    :root {
      --bg: #050816;
      --bg-alt: #0b1020;
      --card: #111827;
      --accent: #38bdf8;
      --accent-soft: rgba(56, 189, 248, 0.12);
      --text: #e5e7eb;
      --text-muted: #9ca3af;
      --border-subtle: #1f2937;
      --danger: #f97373;
      --radius-lg: 18px;
      --radius-pill: 999px;
      --shadow-soft: 0 18px 45px rgba(15, 23, 42, 0.75);
      --shadow-subtle: 0 10px 30px rgba(15, 23, 42, 0.65);
    }

    * {
      box-sizing: border-box;
    }

    html, body {
      margin: 0;
      padding: 0;
      background: radial-gradient(circle at top, #1e293b 0, #020617 55%);
      color: var(--text);
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      scroll-behavior: smooth;
    }

    a {
      color: var(--accent);
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    .page {
      max-width: 1040px;
      margin: 0 auto;
      padding: 32px 20px 60px;
    }

    header {
      display: flex;
      flex-direction: column;
      gap: 18px;
      margin-bottom: 38px;
    }

    @media (min-width: 768px) {
      header {
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
      }
    }

    .brand {
      display: flex;
      flex-direction: column;
      gap: 6px;
    }

    .brand-title {
      font-size: 1.5rem;
      font-weight: 600;
      letter-spacing: 0.04em;
    }

    .brand-subtitle {
      font-size: 0.9rem;
      color: var(--text-muted);
    }

    nav {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-top: 10px;
    }

    .nav-link {
      padding: 7px 14px;
      border-radius: var(--radius-pill);
      border: 1px solid rgba(148, 163, 184, 0.4);
      font-size: 0.8rem;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      color: var(--text-muted);
      text-decoration: none;
    }

    .nav-link:hover {
      border-color: var(--accent);
      color: var(--accent);
    }

    main {
      display: flex;
      flex-direction: column;
      gap: 28px;
    }

    .hero {
      display: grid;
      grid-template-columns: minmax(0, 3fr);
      gap: 20px;
      align-items: center;
      background: linear-gradient(135deg, rgba(15,23,42,0.96), rgba(15,23,42,0.9));
      border-radius: 22px;
      border: 1px solid rgba(148, 163, 184, 0.35);
      box-shadow: var(--shadow-soft);
      padding: 26px 22px 24px;
      position: relative;
      overflow: hidden;
    }

    @media (min-width: 860px) {
      .hero {
        grid-template-columns: minmax(0, 3.2fr) minmax(0, 2.2fr);
        padding: 32px 28px 30px;
      }
    }

    .hero::before {
      content: "";
      position: absolute;
      inset: -40%;
      background: radial-gradient(circle at top right, rgba(56,189,248,0.12), transparent 55%);
      opacity: 0.8;
      pointer-events: none;
    }

    .hero-main {
      position: relative;
      z-index: 1;
    }

    .pill {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 4px 12px;
      border-radius: var(--radius-pill);
      background: rgba(15,23,42,0.9);
      border: 1px solid rgba(148,163,184,0.5);
      color: var(--text-muted);
      font-size: 0.75rem;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      margin-bottom: 12px;
    }

    .pill-dot {
      width: 7px;
      height: 7px;
      border-radius: 999px;
      background: #22c55e;
      box-shadow: 0 0 12px rgba(34, 197, 94, 0.9);
    }

    .hero-title {
      font-size: 1.9rem;
      line-height: 1.15;
      margin: 0 0 12px;
    }

    @media (min-width: 768px) {
      .hero-title {
        font-size: 2.2rem;
      }
    }

    .hero-title span {
      color: var(--accent);
    }

    .hero-tagline {
      font-size: 0.98rem;
      color: var(--text-muted);
      margin-bottom: 16px;
      max-width: 620px;
    }

    .hero-meta {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-bottom: 18px;
    }

    .meta-chip {
      padding: 6px 12px;
      border-radius: var(--radius-pill);
      background: rgba(15,23,42,0.86);
      border: 1px solid rgba(148,163,184,0.45);
      font-size: 0.78rem;
      color: var(--text-muted);
    }

    .meta-chip strong {
      color: var(--text);
      font-weight: 500;
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      padding: 9px 16px;
      border-radius: var(--radius-pill);
      font-size: 0.9rem;
      border: 1px solid transparent;
      cursor: pointer;
      text-decoration: none;
    }

    .btn-primary {
      background: radial-gradient(circle at top left, #38bdf8, #0369a1);
      color: white;
      box-shadow: 0 16px 36px rgba(8, 47, 73, 0.9);
    }

    .btn-primary:hover {
      filter: brightness(1.06);
      text-decoration: none;
    }

    .btn-ghost {
      background: rgba(15,23,42,0.85);
      border-color: rgba(148,163,184,0.6);
      color: var(--text-muted);
    }

    .btn-ghost:hover {
      border-color: var(--accent);
      color: var(--accent);
      text-decoration: none;
    }

    .hero-aside {
      position: relative;
      z-index: 1;
      display: none;
    }

    @media (min-width: 860px) {
      .hero-aside {
        display: block;
      }
    }

    .card {
      background: radial-gradient(circle at top, #111827 0, #020617 70%);
      border-radius: var(--radius-lg);
      padding: 16px 16px 18px;
      border: 1px solid rgba(148,163,184,0.45);
      box-shadow: var(--shadow-subtle);
    }

    .card-heading {
      display: flex;
      justify-content: space-between;
      align-items: baseline;
      margin-bottom: 8px;
    }

    .card-title {
      font-size: 0.9rem;
      font-weight: 500;
    }

    .card-badge {
      font-size: 0.7rem;
      padding: 3px 9px;
      border-radius: var(--radius-pill);
      background: rgba(56,189,248,0.15);
      color: var(--accent);
      border: 1px solid rgba(56,189,248,0.4);
      text-transform: uppercase;
      letter-spacing: 0.12em;
    }

    .tag-cloud {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
      margin: 4px 0 10px;
    }

    .tag {
      font-size: 0.72rem;
      padding: 4px 9px;
      border-radius: var(--radius-pill);
      background: rgba(15,23,42,0.92);
      border: 1px solid rgba(75,85,99,0.9);
      color: var(--text-muted);
    }

    .card-row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      font-size: 0.8rem;
      padding: 6px 0;
      border-top: 1px dashed rgba(55,65,81,0.8);
      margin-top: 4px;
    }

    .card-row span:first-child {
      color: var(--text-muted);
    }

    .badge-severity {
      font-size: 0.7rem;
      padding: 2px 8px;
      border-radius: var(--radius-pill);
      border: 1px solid rgba(148,163,184,0.5);
      color: var(--text-muted);
    }

    .badge-severity.critical {
      border-color: #f97373;
      color: #fecaca;
      background: rgba(248, 113, 113, 0.09);
    }

    .badge-severity.high {
      border-color: #facc15;
      color: #fef9c3;
      background: rgba(234, 179, 8, 0.06);
    }

    .badge-severity.medium {
      border-color: #22c55e;
      color: #bbf7d0;
      background: rgba(34,197,94,0.08);
    }

    .sections {
      display: grid;
      grid-template-columns: minmax(0, 1.9fr) minmax(0, 1.4fr);
      gap: 22px;
    }

    @media (max-width: 880px) {
      .sections {
        grid-template-columns: minmax(0, 1fr);
      }
    }

    .section {
      background: rgba(15, 23, 42, 0.9);
      border-radius: 18px;
      border: 1px solid rgba(30, 64, 175, 0.7);
      box-shadow: var(--shadow-subtle);
      padding: 18px 16px 16px;
    }

    .section h2 {
      font-size: 1.1rem;
      margin-top: 0;
      margin-bottom: 8px;
    }

    .section p {
      font-size: 0.9rem;
      line-height: 1.6;
      color: var(--text-muted);
    }

    .section ul {
      padding-left: 18px;
      margin: 8px 0 4px;
    }

    .section ul li {
      font-size: 0.9rem;
      color: var(--text-muted);
      margin-bottom: 4px;
    }

    .eyebrow {
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.16em;
      color: var(--text-muted);
      margin-bottom: 2px;
    }

    .divider {
      margin: 26px 0 8px;
      border-top: 1px dashed rgba(51,65,85,0.9);
    }

    .artefacts {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 18px;
      margin-top: 10px;
    }

    .artefact-card {
      background: rgba(15,23,42,0.96);
      border-radius: 16px;
      border: 1px solid rgba(55,65,81,0.9);
      padding: 12px 12px 10px;
      display: flex;
      flex-direction: column;
      gap: 6px;
      font-size: 0.86rem;
    }

    .artefact-title {
      font-weight: 500;
    }

    .artefact-meta {
      font-size: 0.78rem;
      color: var(--text-muted);
    }

    .artefact-links a {
      font-size: 0.8rem;
      margin-right: 10px;
    }

    footer {
      margin-top: 36px;
      padding-top: 16px;
      border-top: 1px dashed rgba(51,65,85,0.9);
      font-size: 0.78rem;
      color: var(--text-muted);
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      gap: 8px;
    }
  </style>
</head>
<body>
  <div class="page">
    <header>
      <div class="brand">
        <div class="brand-title">ACEN–UFS merSETA Case Study</div>
        <div class="brand-subtitle">Project Management · Risk Governance · Hybrid PMI / Agile</div>
      </div>
      <nav>
        <a href="#overview" class="nav-link">Overview</a>
        <a href="#risk-governance" class="nav-link">Risk Governance</a>
        <a href="#artefacts" class="nav-link">Artefacts</a>
        <a href="#contact" class="nav-link">About</a>
      </nav>
    </header>

    <main>
      <section class="hero" id="overview">
        <div class="hero-main">
          <div class="pill">
            <span class="pill-dot"></span>
            <span>Project Management Case Study</span>
          </div>
          <h1 class="hero-title">
            Circular Economy Training for South African Manufacturing<br />
            <span>ACEN–UFS–merSETA Programme</span>
          </h1>
          <p class="hero-tagline">
            A national circular economy capacity-building project, managed using a hybrid PMI / Agile approach,
            with a full deliverable-based risk governance system designed and implemented end-to-end.
          </p>
          <div class="hero-meta">
            <div class="meta-chip"><strong>Role:</strong>&nbsp;Project Manager (Hybrid PMI / Scrum)</div>
            <div class="meta-chip"><strong>Domain:</strong>&nbsp;Circular Economy · Skills Development</div>
            <div class="meta-chip"><strong>Focus:</strong>&nbsp;Risk Management · Stakeholder Alignment</div>
          </div>
          <div class="hero-actions">
            <a href="#artefacts" class="btn btn-primary">
              View Risk Register &amp; Files
            </a>
            <a href="#risk-governance" class="btn btn-ghost">
              Read Risk Governance Summary
            </a>
          </div>
        </div>
        <aside class="hero-aside">
          <div class="card">
            <div class="card-heading">
              <div class="card-title">Project Snapshot</div>
              <div class="card-badge">Hybrid PMI / Agile</div>
            </div>
            <div class="tag-cloud">
              <span class="tag">Risk Register (15 Risks)</span>
              <span class="tag">5×5 Heatmap</span>
              <span class="tag">Jira Risk Backlog</span>
              <span class="tag">National CE Programme</span>
            </div>
            <div class="card-row">
              <span>Deliverables</span>
              <span>Desktop Research · Webinars · Training · Case Studies · Close-Out</span>
            </div>
            <div class="card-row">
              <span>Stakeholders</span>
              <span>ACEN · UFS · merSETA · Industry</span>
            </div>
            <div class="card-row">
              <span>Risk Exposure</span>
              <span>
                <span class="badge-severity critical">Critical: 2</span>
                <span class="badge-severity high">High: 6</span>
                <span class="badge-severity medium">Medium: 5</span>
              </span>
            </div>
          </div>
        </aside>
      </section>

      <section class="sections">
        <section class="section">
          <div class="eyebrow">Project context</div>
          <h2>Scope and Objectives</h2>
          <p>
            The ACEN–UFS–merSETA programme aimed to build circular economy capabilities within the South African
            manufacturing ecosystem. The project delivered 15 integrated outputs across desktop research,
            webinar design, training framework development, African and South African case studies, and a
            comprehensive close-out report with recommendations for future CE skills interventions.
          </p>
          <p>
            As Project Manager, I structured the work into six coherent workstreams:
          </p>
          <ul>
            <li>Desktop research on CE actors, programmes, and value chains.</li>
            <li>Webinar design and delivery to introduce CE concepts and opportunities.</li>
            <li>Training frameworks and materials for engineers, manufacturers, and SMME mentors.</li>
            <li>African and South African CE case studies with critical success factors.</li>
            <li>Four live training sessions reaching engineers and SMME mentors.</li>
            <li>Final close-out reporting, lessons learned, and future recommendations.</li>
          </ul>
          <p>
            This required balancing academic expectations, sector authority requirements, and practical constraints
            in a policy-sensitive, data-limited environment.
          </p>
        </section>

        <section class="section" id="risk-governance">
          <div class="eyebrow">Risk governance</div>
          <h2>Hybrid PMI / Agile Risk Management</h2>
          <p>
            I designed a risk management system that combines PMI-style qualitative analysis with Agile delivery practices.
            Each risk is linked to specific deliverables and workstreams and scored using a 5×5 Likelihood × Impact matrix.
          </p>
          <ul>
            <li>Deliverable-based risk register with 15 core risks mapped to C3–C16.</li>
            <li>Qualitative scoring (Low / Medium / High) + numerical severity bands.</li>
            <li>5×5 heatmap for stakeholder-friendly visualisation of exposure.</li>
            <li>Risk stories integrated into the Jira backlog for sprint-level mitigation.</li>
            <li>Early-warning indicators defined for each high-impact risk.</li>
          </ul>
          <p>
            Risks such as data gaps, policy shifts, low training attendance, and restricted case study access
            are prioritised and tracked iteratively, with mitigation work packaged into sprints and reviewed with
            key stakeholders.
          </p>
        </section>
      </section>

      <div class="divider"></div>

      <section class="section" id="artefacts">
        <div class="eyebrow">Deliverables</div>
        <h2>Key Artefacts &amp; Downloads</h2>
        <p>
          The following artefacts are included in this repository to demonstrate end-to-end risk governance on a
          complex, multi-stakeholder project. In an interview or portfolio review, I typically walk through how
          each item fits into the overall governance approach.
        </p>

        <div class="artefacts">
          <div class="artefact-card">
            <div class="artefact-title">Risk Register (Markdown)</div>
            <div class="artefact-meta">
              Human-readable register linking risks to deliverables, owners, and early-warning indicators.
            </div>
            <div class="artefact-links">
              <a href="risk-register.md" target="_blank">Open risk-register.md</a>
            </div>
          </div>

          <div class="artefact-card">
            <div class="artefact-title">Risk Register (Excel Workbook)</div>
            <div class="artefact-meta">
              Excel file with three sheets: Risk Register, Risk Summary (pivot), and Heatmap (5×5 matrix).
            </div>
            <div class="artefact-links">
              <a href="risk-register.xlsx" target="_blank">Download risk-register.xlsx</a>
            </div>
          </div>

          <div class="artefact-card">
            <div class="artefact-title">Risk Register (CSV)</div>
            <div class="artefact-meta">
              Lightweight CSV for import into other tools, BI dashboards, or data analysis notebooks.
            </div>
            <div class="artefact-links">
              <a href="risk-register.csv" target="_blank">Download risk-register.csv</a>
            </div>
          </div>

          <div class="artefact-card">
            <div class="artefact-title">Risk Matrix Heatmap (PNG)</div>
            <div class="artefact-meta">
              5×5 Likelihood × Impact heatmap using a classic green–yellow–red palette for presentations.
            </div>
            <div class="artefact-links">
              <a href="heatmap.png" target="_blank">View heatmap.png</a>
            </div>
          </div>

          <div class="artefact-card">
            <div class="artefact-title">Mermaid Heatmap Snippet</div>
            <div class="artefact-meta">
              Mermaid.js definition for embedding a risk heatmap directly into GitHub or documentation sites.
            </div>
            <div class="artefact-links">
              <a href="mermaid-heatmap.md" target="_blank">Open mermaid-heatmap.md</a>
            </div>
          </div>

          <div class="artefact-card">
            <div class="artefact-title">Jira Risk Backlog (CSV)</div>
            <div class="artefact-meta">
              Importable CSV mapping risks into Jira as “Risk” issues for Agile tracking.
            </div>
            <div class="artefact-links">
              <a href="risk-register-jira-import.csv" target="_blank">Download Jira import CSV</a>
            </div>
          </div>
        </div>
      </section>

      <div class="divider"></div>

      <section class="section" id="contact">
        <div class="eyebrow">About this case study</div>
        <h2>How I Use This in My Practice</h2>
        <p>
          This microsite is part of my project management portfolio. It demonstrates how I apply hybrid PMI and Agile
          methods to real-world, multi-stakeholder programmes in sustainability, research, and training contexts.
        </p>
        <p>
          In conversation with hiring managers or clients, I use this case study to discuss:
        </p>
        <ul>
          <li>How risk governance supports delivery in policy-sensitive environments.</li>
          <li>How I balance academic, regulatory, and operational constraints.</li>
          <li>How I embed risk thinking into Agile cadences (sprints, reviews, retrospectives).</li>
          <li>How tools like Jira, Excel, and visual heatmaps can work together.</li>
        </ul>
        <p>
          You can explore the artefacts above or connect with me directly to talk through the design decisions and
          implementation details behind this system.
        </p>
      </section>
    </main>

    <footer>
      <span>&copy; 2025 ACEN–UFS merSETA Risk Governance Case Study · Created by Jonathan Tager</span>
      <span>Designed for GitHub Pages · Static, no tracking scripts</span>
    </footer>
  </div>
</body>
</html>
