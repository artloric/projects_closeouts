---
layout: page
title: "ACEN Project Case Study"
permalink: /
---

<style>
  :root {
    --acen-teal: #007066;
    --acen-teal-light: #e5f1ef;
    --acen-dark: #20252a;
    --acen-grey: #f5f7f6;
    --accent-gold: #f3b13c;
  }

  body {
    background: var(--acen-grey);
  }

  .hero {
    background: linear-gradient(135deg, var(--acen-teal), #009b8a);
    color: #ffffff;
    padding: 3rem 1.5rem;
    margin: -2rem -1.5rem 2rem;
    text-align: left;
  }

  .hero-inner {
    max-width: 960px;
    margin: 0 auto;
  }

  .hero-title {
    font-size: 2.4rem;
    font-weight: 700;
    margin-bottom: 0.25rem;
  }

  .hero-subtitle {
    font-size: 1.1rem;
    opacity: 0.9;
    margin-bottom: 1rem;
  }

  .hero-meta {
    font-size: 0.95rem;
    opacity: 0.95;
  }

  .hero-badge {
    display: inline-block;
    padding: 0.2rem 0.6rem;
    border-radius: 999px;
    background: rgba(0,0,0,0.2);
    font-size: 0.8rem;
    margin-right: 0.5rem;
  }

  .top-nav {
    background: #ffffff;
    border-radius: 999px;
    box-shadow: 0 10px 25px rgba(0,0,0,0.05);
    width: fit-content;
    max-width: 100%;
    padding: 0.5rem 0.75rem;
    margin: -1.75rem auto 3rem;
    display: flex;
    flex-wrap: wrap;
    gap: 0.25rem;
	
  }

  .top-nav a {
    padding: 0.3rem 0.75rem;
    border-radius: 999px;
    font-size: 0.85rem;
    text-decoration: none;
    color: var(--acen-dark);
    white-space: nowrap;
  }

  .top-nav a:hover {
    background: var(--acen-teal-light);
    color: var(--acen-teal);
  }

  .top-nav a.nav-primary {
    background: var(--acen-teal);
    color: #ffffff;
  }

  .page-content {
    max-width: 960px;
    margin: 0 auto;
  }

  section {
    margin-bottom: 3rem;
    background: #ffffff;
    padding: 1.75rem 1.5rem;
    border-radius: 1rem;
    box-shadow: 0 6px 18px rgba(0,0,0,0.03);
  }

  section h2 {
    color: var(--acen-teal);
    border-bottom: 2px solid var(--acen-teal-light);
    padding-bottom: 0.4rem;
    margin-bottom: 1rem;
    font-size: 1.35rem;
  }

  section h3 {
    color: var(--acen-dark);
    font-size: 1.05rem;
    margin-top: 1.1rem;
  }

  .meta-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(210px, 1fr));
    gap: 0.75rem 1.5rem;
    margin-top: 0.75rem;
  }

  .meta-item-label {
    font-size: 0.8rem;
    text-transform: uppercase;
    letter-spacing: 0.08em;
    color: #666;
  }

  .meta-item-value {
    font-size: 0.95rem;
    color: var(--acen-dark);
  }

  table {
    width: 100%;
    border-collapse: collapse;
    font-size: 0.9rem;
    margin-top: 0.75rem;
  }

  th, td {
    border: 1px solid #e2e4e8;
    padding: 0.45rem 0.6rem;
    vertical-align: top;
  }

  th {
    background: var(--acen-teal-light);
    color: var(--acen-dark);
    font-weight: 600;
  }

  tbody tr:nth-child(even) td {
    background: #fafbfb;
  }

  .tag-row span {
    display: inline-block;
    padding: 0.2rem 0.55rem;
    border-radius: 999px;
    background: #eef0f2;
    font-size: 0.8rem;
    margin-right: 0.25rem;
    margin-bottom: 0.25rem;
  }

  .pill {
    display: inline-block;
    padding: 0.15rem 0.55rem;
    border-radius: 999px;
    border: 1px solid #d0d4d7;
    font-size: 0.78rem;
    margin: 0.12rem 0.12rem 0 0;
  }

  .pill.on {
    background: var(--acen-teal-light);
    border-color: var(--acen-teal);
    color: var(--acen-teal);
  }

  .cv-highlight {
    border-left: 4px solid var(--accent-gold);
    padding-left: 0.75rem;
    margin-top: 0.75rem;
  }

  @media (max-width: 600px) {
    .hero {
      margin: -1.5rem -1rem 1.5rem;
    }
    section {
      padding: 1.25rem 1rem;
      border-radius: 0.75rem;
    }
  }
</style>

<div class="hero">
  <div class="hero-inner">
    <div class="hero-badge">ACEN Project Close-Out</div>
    <div class="hero-title">Project Title Goes Here</div>
    <div class="hero-subtitle">
      Short one-line tagline describing the project and its purpose.
    </div>
    <div class="hero-meta">
      <strong>Client / Partner:</strong> [Insert Partner] &nbsp; | &nbsp;
      <strong>Duration:</strong> [e.g. Jan 2024 – Sep 2024] &nbsp; | &nbsp;
      <strong>Lead:</strong> [Your Name]
    </div>
  </div>
</div>

<div class="top-nav">
  <a href="#overview" class="nav-primary">Overview</a>
  <a href="#scope">Scope &amp; Objectives</a>
  <a href="#deliverables">Deliverables</a>
  <a href="#outcomes">Outcomes</a>
  <a href="#impact-map">Impact Map</a>
  <a href="#challenges">Challenges</a>
  <a href="#lessons">Lessons</a>
  <a href="#recommendations">Recommendations</a>
  <a href="#contribution">Personal Contribution</a>
</div>

<div class="page-content">

<section id="overview">
  <h2>1. Project Overview</h2>

  <h3>1.1 Project Profile</h3>
  <div class="meta-grid">
    <div>
      <div class="meta-item-label">Project Name</div>
      <div class="meta-item-value">[Insert project name]</div>
    </div>
    <div>
      <div class="meta-item-label">Client / Partner</div>
      <div class="meta-item-value">[e.g. UFS, merSETA]</div>
    </div>
    <div>
      <div class="meta-item-label">Implementing Organisation</div>
      <div class="meta-item-value">African Circular Economy Network (ACEN)</div>
    </div>
    <div>
      <div class="meta-item-label">Project Manager / Lead Analyst</div>
      <div class="meta-item-value">[Your name]</div>
    </div>
    <div>
      <div class="meta-item-label">Duration</div>
      <div class="meta-item-value">[Dates]</div>
    </div>
    <div>
      <div class="meta-item-label">Project Type</div>
      <div class="meta-item-value">
        <span class="pill on">Research &amp; Analysis</span>
        <span class="pill">Training</span>
        <span class="pill">Curriculum Development</span>
        <span class="pill">Case Studies</span>
        <span class="pill">Advisory</span>
        <span class="pill">Hybrid</span>
      </div>
    </div>
  </div>

  <h3>1.2 Project Purpose</h3>
  <p>
    Briefly describe <strong>why</strong> this project existed, the problem it addressed,
    and its strategic importance for the client, South Africa’s CE transition, and ACEN’s mission.
  </p>

  <div class="cv-highlight">
    <strong>Executive Summary (portfolio-friendly):</strong><br>
    In 3–5 lines, summarise the project goals, what you delivered, and the impact.
  </div>
</section>

<section id="scope">
  <h2>2. Scope, Objectives &amp; Approach</h2>

  <h3>2.1 Objectives</h3>
  <p>Select and adapt as needed:</p>
  <ul>
    <li>Conduct foundational circular economy (CE) research and ecosystem mapping (C3.1–C3.3).</li>
    <li>Develop CE awareness training and webinars.</li>
    <li>Create training frameworks for Engineers &amp; Manufacturers and SMME Mentors.</li>
    <li>Design and deliver CE training sessions to targeted cohorts.</li>
    <li>Identify, research, and document African CE case studies.</li>
    <li>Produce a comprehensive post-project evaluation and close-out report.</li>
  </ul>

  <h3>2.2 Approach &amp; Methodology</h3>
  <p>
    Describe the combination of <strong>research methods</strong>, <strong>training design logic</strong>, and
    <strong>project management approach</strong> you used. For example:
  </p>
  <ul>
    <li>Desktop research, literature review, and synthesis of policy and technical reports.</li>
    <li>Training design using Bloom’s Taxonomy and NQF alignment.</li>
    <li>Case study selection and analysis based on predefined CE criteria.</li>
    <li>Agile-style iteration with frequent alignment check-ins and versioning.</li>
  </ul>
</section>

<section id="deliverables">
  <h2>3. Deliverables Completed</h2>

  <h3>3.1 Deliverables Summary</h3>

  | Deliverable | Title / Description | Status | Notes |
  |-------------|---------------------|--------|-------|
  | C3.1 | Desktop research on CE structures, programmes, and actors | Delivered | Informed training design |
  | C3.2 | CE research opportunities &amp; training requirements | Delivered | |
  | C3.3 | CE case study opportunity identification | Delivered | |
  | C4.1 | CE Awareness Webinars (x3) | Delivered | Drafts aligned with UFS |
  | C5.1 | Training framework for Engineers &amp; Manufacturers | Delivered | |
  | C5.2 | Training framework for SMME Mentors | Delivered | |
  | C8–C10 | CE case study development | Delivered | |
  | C11–C15 | Training sessions | Delivered | e.g. 40 participants each |
  | C16 | Project close-out report | Delivered | This case study |

  <h3>3.2 Tools, Systems &amp; Frameworks</h3>
  <p><strong>Project Tools:</strong> Notion, Miro, MS Teams, SharePoint, Excel, Word, WhatsApp.</p>
  <p><strong>Frameworks:</strong> Bloom’s Taxonomy, CE principles (EMF, ISO 59020), systems thinking, R-ladder &amp; CE loops, value chain analysis, theory of change.</p>
</section>

<section id="outcomes">
  <h2>4. Project Performance &amp; Outcomes</h2>

  <h3>4.1 Key Achievements</h3>
  <ul>
    <li>Summarise 4–6 key achievements (e.g. completed research, training frameworks, webinars, case studies).</li>
    <li>Emphasise how these deliverables support the client’s strategic goals and CE transition.</li>
  </ul>

  <h3>4.2 Quantitative Indicators</h3>

  | Indicator | Value |
  |----------|-------|
  | Deliverables completed | |
  | Stakeholders identified / mapped | |
  | Training sessions delivered | |
  | Participants trained | |
  | Case studies documented | |

  <h3>4.3 Value Delivered</h3>
  <p>
    Explain the qualitative value delivered to:
  </p>
  <ul>
    <li><strong>Client:</strong> clearer CE roadmap, training assets, research base.</li>
    <li><strong>Sector:</strong> evidence for CE skills gaps and interventions.</li>
    <li><strong>ACEN:</strong> reusable frameworks, templates, and credibility in CE training and research.</li>
  </ul>
</section>

<section id="impact-map">
  <h2>5. Impact &amp; Logic Model</h2>

  <p>
    This diagram summarises how project <strong>inputs</strong> and <strong>activities</strong>
    translated into <strong>outputs</strong>, <strong>outcomes</strong>, and longer-term
    <strong>impact</strong> for ACEN, the client, and the wider CE ecosystem.
  </p>

```mermaid
flowchart LR
    subgraph Inputs
        I1(Funding &amp; mandate)<br/>(merSETA / UFS)
        I2(ACEN expertise)<br/>(research &amp; CE practice)
        I3(Existing CE policy &amp; literature)
        I4(Stakeholder networks)<br/>(industry, SMMEs, CE actors)
    end

    subgraph Activities
        A1(Desktop research &amp;<br/>ecosystem mapping)
        A2(Training design using<br/>Bloom's Taxonomy &amp; NQF)
        A3(Case study selection &amp;<br/>analysis)
        A4(Stakeholder engagement &amp;<br/>alignment workshops)
        A5(Delivery of webinars &amp;<br/>training sessions)
    end

    subgraph Outputs
        O1(Research reports<br/>(C3.1–C3.3))
        O2(Training frameworks &amp;<br/>curricula (C5–C6))
        O3(Webinars &amp; training<br/>materials (C4, C11–C15))
        O4(Case study compendium<br/>(C8–C10))
        O5(Project close-out &amp;<br/>evaluation (C16))
    end

    subgraph Outcomes
        OC1(Improved CE awareness<br/>among engineers &amp; SMME mentors)
        OC2(Clearer view of CE actors,<br/>gaps, and opportunities)
        OC3(Reusable CE training assets<br/>for future cohorts)
        OC4(Stronger positioning of ACEN<br/>as CE knowledge partner)
    end

    subgraph Impact
        IM1(Contribution to South Africa's<br/>CE skills pipeline)
        IM2(Better-informed policy &amp;<br/>programme design)
        IM3(Scaling potential of CE training<br/>across sectors &amp; geographies)
    end

    Inputs --> Activities --> Outputs --> Outcomes --> Impact

    I1 --> A1
    I2 --> A2
    I3 --> A1
    I4 --> A4

    A1 --> O1
    A2 --> O2
    A3 --> O4
    A4 --> O5
    A5 --> O3

    O1 --> OC2
    O2 --> OC3
    O3 --> OC1
    O4 --> OC2
    O5 --> OC4

    OC1 --> IM1
    OC2 --> IM2
    OC3 --> IM1
    OC4 --> IM3
```

<section id="challenges">
  <h2>5. Challenges &amp; Mitigation</h2>

  <h3>5.1 Key Challenges</h3>
  <ul>
    <li>Ambiguous or evolving ToR at project start.</li>
    <li>Limited existing CE training ecosystem in South Africa.</li>
    <li>Data scarcity or fragmentation for African CE case studies.</li>
    <li>Tight timelines and multi-stakeholder coordination.</li>
  </ul>

  <h3>5.2 Mitigation Strategies</h3>
  <ul>
    <li>Used iterative alignment sessions to refine scope and expectations.</li>
    <li>Applied structured frameworks to bring clarity to complex content.</li>
    <li>Maintained frequent communication with UFS, merSETA, and ACEN leadership.</li>
    <li>Prioritised deliverables and used version control for transparency.</li>
  </ul>
</section>

<section id="lessons">
  <h2>6. Lessons Learned</h2>

  <h3>6.1 Project Delivery</h3>
  <ul>
    <li>Early scoping alignment is essential for multi-deliverable research &amp; training projects.</li>
    <li>Version control and regular check-ins reduce rework and misunderstandings.</li>
  </ul>

  <h3>6.2 Sectoral (Manufacturing / SMMEs / CE)</h3>
  <ul>
    <li>Foundational CE training is still scarce; there is strong demand across the ecosystem.</li>
    <li>SMMEs need tailored CE business model support and accessible language.</li>
  </ul>

  <h3>6.3 Organisational (ACEN)</h3>
  <ul>
    <li>Reusable frameworks and templates significantly reduce effort for future projects.</li>
    <li>A centralised CE knowledge base (actors, policies, interventions) increases ACEN’s leverage.</li>
  </ul>
</section>

<section id="recommendations">
  <h2>7. Recommendations for Future Projects</h2>

  <ul>
    <li>Adopt a phased impact evaluation model (baseline → post-training → 6–9 month follow-up).</li>
    <li>Update the CE ecosystem map annually to reflect new actors and policies.</li>
    <li>Expand partnerships with TVETs, SEZs, and SETAs to embed CE curricula.</li>
    <li>Pursue demonstration projects to de-risk CE interventions and attract further investment.</li>
  </ul>
</section>

<section id="contribution">
  <h2>8. Personal Contribution Summary (CV-Ready)</h2>

  <h3>Role</h3>
  <p>Project Manager / Lead Analyst (or your title)</p>

  <h3>Key Contributions</h3>
  <ul>
    <li>Led a multi-deliverable CE programme (C3–C16) from inception to close-out.</li>
    <li>Designed and structured CE training frameworks using Bloom’s Taxonomy and NQF alignment.</li>
    <li>Coordinated research synthesis across policy, technical reports, and stakeholder inputs.</li>
    <li>Managed stakeholder engagement with UFS, merSETA, ACEN directors, and CE practitioners.</li>
    <li>Ensured quality control, version management, and timely delivery of all outputs.</li>
  </ul>

  <h3>Skills Demonstrated</h3>
  <div class="tag-row">
    <span>Strategic &amp; analytical thinking</span>
    <span>Agile project management</span>
    <span>Systems &amp; design thinking</span>
    <span>Research design &amp; synthesis</span>
    <span>Curriculum &amp; training design</span>
    <span>Stakeholder communication</span>
  </div>
</section>

<section id="appendices">
  <h2>9. Appendices (Optional)</h2>
  <ul>
    <li>Appendix A: Detailed Deliverables Matrix</li>
    <li>Appendix B: Hours Log / Effort Breakdown</li>
    <li>Appendix C: Stakeholder Engagement Summary</li>
    <li>Appendix D: Training Feedback &amp; Evaluation Results</li>
    <li>Appendix E: Risk Register</li>
  </ul>
</section>

</div>
