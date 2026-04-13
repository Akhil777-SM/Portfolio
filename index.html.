<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Akhil C A — Social Media Manager</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;1,300;1,400&family=Jost:wght@200;300;400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --ink: #0e0d0b;
    --cream: #f5f0e8;
    --gold: #c9a84c;
    --gold-light: #e8c97a;
    --warm-gray: #6b6560;
    --section-bg: #faf8f4;
    --card-bg: #ffffff;
    --border: rgba(201,168,76,0.25);
    --border-light: rgba(201,168,76,0.12);
  }

  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  html { scroll-behavior: smooth; font-size: 16px; }

  body {
    font-family: 'Jost', sans-serif;
    background: var(--cream);
    color: var(--ink);
    line-height: 1.7;
    overflow-x: hidden;
  }

  /* ─── SCROLLBAR ─── */
  ::-webkit-scrollbar { width: 4px; }
  ::-webkit-scrollbar-track { background: var(--cream); }
  ::-webkit-scrollbar-thumb { background: var(--gold); border-radius: 2px; }

  /* ─── NAV ─── */
  nav {
    position: fixed; top: 0; left: 0; right: 0; z-index: 100;
    display: flex; align-items: center; justify-content: space-between;
    padding: 1.4rem 5vw;
    background: rgba(245,240,232,0.88);
    backdrop-filter: blur(12px);
    border-bottom: 1px solid var(--border-light);
    transition: all 0.3s ease;
  }
  .nav-logo {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.35rem; font-weight: 500; letter-spacing: 0.05em;
    color: var(--ink); text-decoration: none;
  }
  .nav-logo span { color: var(--gold); }
  .nav-links { display: flex; gap: 2rem; list-style: none; }
  .nav-links a {
    font-size: 0.72rem; letter-spacing: 0.15em; text-transform: uppercase;
    color: var(--warm-gray); text-decoration: none; font-weight: 400;
    transition: color 0.2s;
  }
  .nav-links a:hover { color: var(--gold); }
  .nav-cta {
    font-size: 0.7rem; letter-spacing: 0.18em; text-transform: uppercase;
    font-weight: 500; color: var(--gold); text-decoration: none;
    border: 1px solid var(--gold); padding: 0.55rem 1.3rem;
    transition: all 0.25s ease;
  }
  .nav-cta:hover { background: var(--gold); color: var(--cream); }

  /* ─── HERO ─── */
  #hero {
    min-height: 100vh;
    display: grid; grid-template-columns: 1fr 1fr;
    align-items: center;
    padding: 8rem 5vw 5rem;
    background: var(--ink);
    position: relative; overflow: hidden;
  }
  .hero-grain {
    position: absolute; inset: 0; z-index: 0;
    background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 512 512' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.75' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.04'/%3E%3C/svg%3E");
    opacity: 0.6; pointer-events: none;
  }
  .hero-line-deco {
    position: absolute; top: 0; right: 40%; width: 1px; height: 100%;
    background: linear-gradient(to bottom, transparent, var(--gold) 30%, var(--gold) 70%, transparent);
    opacity: 0.15;
  }
  .hero-content { position: relative; z-index: 1; }
  .hero-eyebrow {
    font-size: 0.68rem; letter-spacing: 0.3em; text-transform: uppercase;
    color: var(--gold); margin-bottom: 1.8rem; font-weight: 400;
    display: flex; align-items: center; gap: 1rem;
  }
  .hero-eyebrow::before {
    content: ''; display: block; width: 40px; height: 1px; background: var(--gold);
  }
  h1.hero-name {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(3.5rem, 7vw, 6rem);
    font-weight: 300; line-height: 1.05;
    color: var(--cream); margin-bottom: 0.4rem;
  }
  h1.hero-name em { font-style: italic; color: var(--gold); }
  .hero-title {
    font-size: 0.78rem; letter-spacing: 0.25em; text-transform: uppercase;
    color: rgba(245,240,232,0.45); margin-bottom: 2.4rem; font-weight: 300;
  }
  .hero-desc {
    font-size: 1rem; color: rgba(245,240,232,0.65); font-weight: 300;
    max-width: 420px; line-height: 1.8; margin-bottom: 3rem;
  }
  .hero-actions { display: flex; gap: 1.2rem; align-items: center; }
  .btn-primary {
    background: var(--gold); color: var(--ink);
    font-size: 0.7rem; letter-spacing: 0.2em; text-transform: uppercase;
    font-weight: 500; padding: 0.85rem 2.2rem; text-decoration: none;
    font-family: 'Jost', sans-serif;
    transition: all 0.25s ease;
  }
  .btn-primary:hover { background: var(--gold-light); }
  .btn-ghost {
    color: rgba(245,240,232,0.6);
    font-size: 0.7rem; letter-spacing: 0.2em; text-transform: uppercase;
    font-weight: 400; text-decoration: none; border-bottom: 1px solid rgba(245,240,232,0.2);
    padding-bottom: 2px; transition: all 0.25s ease;
  }
  .btn-ghost:hover { color: var(--gold); border-color: var(--gold); }
  .hero-right {
    position: relative; z-index: 1;
    display: flex; flex-direction: column; align-items: flex-end; gap: 1.5rem;
  }
  .hero-stats {
    display: grid; grid-template-columns: 1fr 1fr; gap: 1px;
    border: 1px solid rgba(201,168,76,0.2); width: 100%; max-width: 380px;
  }
  .stat-cell {
    padding: 2rem 1.8rem;
    border: 1px solid rgba(201,168,76,0.12);
    background: rgba(255,255,255,0.02);
    transition: background 0.3s;
  }
  .stat-cell:hover { background: rgba(201,168,76,0.06); }
  .stat-num {
    font-family: 'Cormorant Garamond', serif;
    font-size: 2.8rem; font-weight: 300;
    color: var(--gold); line-height: 1;
    margin-bottom: 0.4rem;
  }
  .stat-label {
    font-size: 0.65rem; letter-spacing: 0.2em; text-transform: uppercase;
    color: rgba(245,240,232,0.4); font-weight: 300;
  }
  .hero-location {
    font-size: 0.68rem; letter-spacing: 0.2em; text-transform: uppercase;
    color: rgba(245,240,232,0.3); align-self: flex-end;
  }

  /* ─── SECTION SHELL ─── */
  section { padding: 7rem 5vw; }
  .section-tag {
    font-size: 0.65rem; letter-spacing: 0.3em; text-transform: uppercase;
    color: var(--gold); margin-bottom: 1rem; font-weight: 400;
    display: flex; align-items: center; gap: 0.8rem;
  }
  .section-tag::before { content:''; display:block; width:28px; height:1px; background:var(--gold); }
  h2.section-title {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(2.2rem, 4vw, 3.4rem);
    font-weight: 300; line-height: 1.1; color: var(--ink);
    margin-bottom: 3.5rem;
  }
  h2.section-title em { font-style: italic; color: var(--gold); }
  .divider { width: 60px; height: 1px; background: var(--gold); margin: 2rem 0; opacity: 0.5; }

  /* ─── ABOUT ─── */
  #about { background: var(--section-bg); }
  .about-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 6rem; align-items: start; }
  .about-body p {
    font-size: 1rem; color: var(--warm-gray); font-weight: 300; line-height: 1.9;
    margin-bottom: 1.4rem;
  }
  .about-body p strong { color: var(--ink); font-weight: 500; }
  .about-body p em { font-family: 'Cormorant Garamond', serif; font-size: 1.1rem; font-style: italic; color: var(--gold); }
  .about-highlights { display: flex; flex-direction: column; gap: 1.5rem; }
  .highlight-item {
    padding: 1.8rem 2rem;
    border: 1px solid var(--border);
    background: var(--card-bg);
    transition: box-shadow 0.3s;
    position: relative;
  }
  .highlight-item::before {
    content: ''; position: absolute; top: 0; left: 0;
    width: 3px; height: 0; background: var(--gold);
    transition: height 0.35s ease;
  }
  .highlight-item:hover::before { height: 100%; }
  .highlight-item:hover { box-shadow: 0 8px 40px rgba(0,0,0,0.06); }
  .hi-icon { font-size: 1.3rem; margin-bottom: 0.6rem; }
  .hi-title { font-size: 0.75rem; letter-spacing: 0.15em; text-transform: uppercase; font-weight: 500; color: var(--ink); margin-bottom: 0.4rem; }
  .hi-text { font-size: 0.88rem; color: var(--warm-gray); font-weight: 300; }

  /* ─── EXPERIENCE ─── */
  #experience { background: var(--ink); }
  #experience .section-tag { color: var(--gold-light); }
  #experience h2.section-title { color: var(--cream); }
  .timeline { position: relative; padding-left: 2.5rem; }
  .timeline::before {
    content: ''; position: absolute; left: 0; top: 0.5rem; bottom: 0;
    width: 1px; background: linear-gradient(to bottom, var(--gold), transparent);
    opacity: 0.3;
  }
  .timeline-item {
    position: relative; margin-bottom: 4rem; padding-left: 1.5rem;
  }
  .timeline-item::before {
    content: ''; position: absolute; left: -2.5rem; top: 0.45rem;
    width: 8px; height: 8px; border: 1px solid var(--gold);
    background: var(--ink); border-radius: 50%;
  }
  .timeline-period {
    font-size: 0.65rem; letter-spacing: 0.25em; text-transform: uppercase;
    color: var(--gold); margin-bottom: 0.6rem; font-weight: 400;
  }
  .timeline-role {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.6rem; font-weight: 400; color: var(--cream);
    margin-bottom: 0.2rem;
  }
  .timeline-company {
    font-size: 0.78rem; letter-spacing: 0.12em; text-transform: uppercase;
    color: rgba(245,240,232,0.4); margin-bottom: 1.4rem;
  }
  .timeline-bullets { list-style: none; }
  .timeline-bullets li {
    font-size: 0.92rem; color: rgba(245,240,232,0.6); font-weight: 300;
    line-height: 1.7; margin-bottom: 0.6rem; padding-left: 1.2rem; position: relative;
  }
  .timeline-bullets li::before {
    content: '—'; position: absolute; left: 0; color: var(--gold); opacity: 0.7;
  }

  /* ─── CASE STUDIES ─── */
  #case-studies { background: var(--cream); }
  .cases-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 2px; }
  .case-card {
    background: var(--card-bg);
    padding: 2.5rem 2rem;
    border: 1px solid var(--border-light);
    position: relative; overflow: hidden;
    transition: all 0.35s ease;
  }
  .case-card::after {
    content: ''; position: absolute; inset: 0;
    background: linear-gradient(135deg, rgba(201,168,76,0.04), transparent);
    opacity: 0; transition: opacity 0.35s;
  }
  .case-card:hover { transform: translateY(-4px); box-shadow: 0 20px 60px rgba(0,0,0,0.08); }
  .case-card:hover::after { opacity: 1; }
  .case-number {
    font-family: 'Cormorant Garamond', serif;
    font-size: 3rem; font-weight: 300; color: rgba(201,168,76,0.15);
    line-height: 1; margin-bottom: 1.4rem;
  }
  .case-brand {
    font-size: 0.68rem; letter-spacing: 0.25em; text-transform: uppercase;
    color: var(--gold); margin-bottom: 0.4rem; font-weight: 500;
  }
  .case-title {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.3rem; font-weight: 400; color: var(--ink);
    margin-bottom: 1rem; line-height: 1.3;
  }
  .case-body { font-size: 0.88rem; color: var(--warm-gray); font-weight: 300; line-height: 1.7; margin-bottom: 1.5rem; }
  .case-metric {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.8rem; font-weight: 300; color: var(--gold);
    display: block; margin-bottom: 0.1rem;
  }
  .case-metric-label { font-size: 0.65rem; letter-spacing: 0.2em; text-transform: uppercase; color: var(--warm-gray); }

  /* ─── SKILLS ─── */
  #skills { background: var(--section-bg); }
  .skills-wrapper { display: grid; grid-template-columns: repeat(2, 1fr); gap: 3rem; }
  .skill-category { }
  .skill-cat-title {
    font-size: 0.68rem; letter-spacing: 0.25em; text-transform: uppercase;
    color: var(--gold); margin-bottom: 1.6rem; font-weight: 500;
  }
  .skill-bars { display: flex; flex-direction: column; gap: 1.1rem; }
  .skill-bar-item { }
  .skill-bar-head {
    display: flex; justify-content: space-between;
    font-size: 0.82rem; color: var(--ink); font-weight: 400;
    margin-bottom: 0.45rem;
  }
  .skill-bar-pct { color: var(--warm-gray); font-size: 0.75rem; }
  .skill-bar-track {
    height: 2px; background: rgba(201,168,76,0.15); position: relative; overflow: hidden;
  }
  .skill-bar-fill {
    height: 100%; background: var(--gold); position: absolute; left: 0; top: 0;
    transform-origin: left; animation: barGrow 1.2s ease forwards;
    transform: scaleX(0);
  }
  @keyframes barGrow { to { transform: scaleX(1); } }

  /* ─── TOOLS ─── */
  #tools { background: var(--ink); }
  #tools .section-tag { color: var(--gold-light); }
  #tools h2.section-title { color: var(--cream); }
  .tools-grid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 2px; }
  .tool-chip {
    padding: 1.6rem 1.4rem;
    border: 1px solid rgba(201,168,76,0.12);
    text-align: center;
    transition: all 0.25s;
    cursor: default;
  }
  .tool-chip:hover { border-color: var(--gold); background: rgba(201,168,76,0.06); }
  .tool-icon { font-size: 1.6rem; margin-bottom: 0.6rem; display: block; }
  .tool-name {
    font-size: 0.72rem; letter-spacing: 0.12em; text-transform: uppercase;
    color: rgba(245,240,232,0.55); font-weight: 300;
  }
  .tool-cat-label {
    font-size: 0.58rem; letter-spacing: 0.2em; text-transform: uppercase;
    color: var(--gold); margin-top: 0.3rem; display: block;
  }

  /* ─── CERTIFICATIONS ─── */
  #certifications { background: var(--cream); }
  .certs-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 2rem; }
  .cert-card {
    display: flex; gap: 1.5rem; padding: 2rem 2rem;
    border: 1px solid var(--border);
    background: var(--card-bg);
    align-items: flex-start; transition: all 0.3s ease;
    position: relative;
  }
  .cert-card:hover { box-shadow: 0 12px 40px rgba(201,168,76,0.1); border-color: var(--gold); }
  .cert-badge {
    flex-shrink: 0; width: 50px; height: 50px;
    border: 1px solid var(--border); display: flex; align-items: center; justify-content: center;
    font-size: 1.4rem;
  }
  .cert-body { }
  .cert-issuer {
    font-size: 0.62rem; letter-spacing: 0.2em; text-transform: uppercase;
    color: var(--gold); margin-bottom: 0.3rem;
  }
  .cert-name {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.15rem; font-weight: 400; color: var(--ink); margin-bottom: 0.4rem;
  }
  .cert-desc { font-size: 0.82rem; color: var(--warm-gray); font-weight: 300; line-height: 1.6; }

  /* ─── EDUCATION ─── */
  #education { background: var(--section-bg); }
  .edu-block {
    display: grid; grid-template-columns: 1fr 2fr; gap: 4rem; align-items: start;
    border: 1px solid var(--border);
    padding: 3rem;
    background: var(--card-bg);
    max-width: 860px;
  }
  .edu-year {
    font-family: 'Cormorant Garamond', serif;
    font-size: 4rem; font-weight: 300; color: rgba(201,168,76,0.2);
    line-height: 1;
  }
  .edu-degree {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.9rem; font-weight: 300; color: var(--ink);
    margin-bottom: 0.5rem;
  }
  .edu-inst {
    font-size: 0.7rem; letter-spacing: 0.2em; text-transform: uppercase;
    color: var(--gold); margin-bottom: 1rem;
  }
  .edu-note { font-size: 0.88rem; color: var(--warm-gray); font-weight: 300; line-height: 1.7; }

  /* ─── CONTACT ─── */
  #contact { background: var(--ink); }
  #contact .section-tag { color: var(--gold-light); }
  #contact h2.section-title { color: var(--cream); }
  .contact-layout { display: grid; grid-template-columns: 1fr 1fr; gap: 6rem; align-items: start; }
  .contact-intro {
    font-size: 1rem; color: rgba(245,240,232,0.55); font-weight: 300; line-height: 1.9;
    margin-bottom: 2.5rem;
  }
  .contact-details { display: flex; flex-direction: column; gap: 1.5rem; }
  .contact-item { display: flex; gap: 1.2rem; align-items: flex-start; }
  .contact-icon { font-size: 1rem; margin-top: 0.1rem; opacity: 0.5; }
  .contact-label {
    font-size: 0.62rem; letter-spacing: 0.2em; text-transform: uppercase;
    color: var(--gold); margin-bottom: 0.15rem;
  }
  .contact-value {
    font-size: 0.95rem; color: rgba(245,240,232,0.75); font-weight: 300;
  }
  .contact-value a { color: inherit; text-decoration: none; transition: color 0.2s; }
  .contact-value a:hover { color: var(--gold-light); }
  .contact-availability {
    padding: 2rem 2.5rem;
    border: 1px solid rgba(201,168,76,0.2);
    background: rgba(255,255,255,0.02);
    margin-top: 2rem;
  }
  .avail-dot {
    width: 8px; height: 8px; border-radius: 50%; background: #6bcf7f;
    display: inline-block; margin-right: 0.6rem;
    animation: pulse 2s infinite;
  }
  @keyframes pulse {
    0%, 100% { opacity: 1; }
    50% { opacity: 0.4; }
  }
  .avail-text {
    font-size: 0.72rem; letter-spacing: 0.18em; text-transform: uppercase;
    color: rgba(245,240,232,0.5);
  }
  .contact-cta-block { display: flex; flex-direction: column; justify-content: center; }
  .large-cta {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(2rem, 4vw, 3rem); font-weight: 300; font-style: italic;
    color: rgba(245,240,232,0.15); line-height: 1.2; margin-bottom: 2.5rem;
  }
  .large-cta strong { color: rgba(245,240,232,0.5); font-style: normal; font-weight: 300; }

  /* ─── FOOTER ─── */
  footer {
    padding: 2rem 5vw;
    background: var(--ink);
    border-top: 1px solid rgba(201,168,76,0.1);
    display: flex; justify-content: space-between; align-items: center;
  }
  .footer-name {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1rem; color: rgba(245,240,232,0.3);
  }
  .footer-note {
    font-size: 0.65rem; letter-spacing: 0.18em; text-transform: uppercase;
    color: rgba(245,240,232,0.2);
  }

  /* ─── REVEAL ANIMATION ─── */
  .reveal {
    opacity: 0; transform: translateY(28px);
    transition: opacity 0.7s ease, transform 0.7s ease;
  }
  .reveal.visible { opacity: 1; transform: translateY(0); }
  .reveal-delay-1 { transition-delay: 0.1s; }
  .reveal-delay-2 { transition-delay: 0.2s; }
  .reveal-delay-3 { transition-delay: 0.32s; }
  .reveal-delay-4 { transition-delay: 0.44s; }
  .reveal-delay-5 { transition-delay: 0.56s; }

  /* ─── RESPONSIVE ─── */
  @media (max-width: 900px) {
    #hero { grid-template-columns: 1fr; padding: 7rem 5vw 4rem; }
    .hero-right { display: none; }
    .about-grid, .contact-layout { grid-template-columns: 1fr; gap: 3rem; }
    .cases-grid { grid-template-columns: 1fr 1fr; }
    .tools-grid { grid-template-columns: repeat(3, 1fr); }
    .skills-wrapper { grid-template-columns: 1fr; }
    .certs-grid { grid-template-columns: 1fr; }
    .edu-block { grid-template-columns: 1fr; gap: 1.5rem; }
    .edu-year { font-size: 2.5rem; }
  }
  @media (max-width: 600px) {
    nav .nav-links { display: none; }
    .cases-grid { grid-template-columns: 1fr; }
    .tools-grid { grid-template-columns: repeat(2, 1fr); }
  }
</style>
</head>
<body>

<!-- NAV -->
<nav>
  <a href="#hero" class="nav-logo">Akhil <span>C A</span></a>
  <ul class="nav-links">
    <li><a href="#about">About</a></li>
    <li><a href="#experience">Experience</a></li>
    <li><a href="#case-studies">Work</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#tools">Tools</a></li>
    <li><a href="#certifications">Certifications</a></li>
  </ul>

</nav>

<!-- ── 1. HERO ── -->
<section id="hero">
  <div class="hero-grain"></div>
  <div class="hero-line-deco"></div>

  <div class="hero-content">
    <div class="hero-eyebrow">Social Media Manager</div>
    <h1 class="hero-name">Akhil<br><em>C A</em></h1>
    <p class="hero-title">Kochi, India &nbsp;·&nbsp; Meta &amp; Google Ads Specialist</p>
    <p class="hero-desc">
      Performance-driven strategist with 3+ years crafting paid social campaigns, 
      organic content ecosystems, and data-backed growth strategies for 10+ brands across India.
    </p>
    <div class="hero-actions">
      <a href="#case-studies" class="btn-primary">View My Work</a>
      <a href="#contact" class="btn-ghost">Get In Touch →</a>
    </div>
  </div>

  <div class="hero-right">
    <div class="hero-stats">
      <div class="stat-cell">
        <div class="stat-num">3+</div>
        <div class="stat-label">Years Experience</div>
      </div>
      <div class="stat-cell">
        <div class="stat-num">10+</div>
        <div class="stat-label">Clients Managed</div>
      </div>
      <div class="stat-cell">
        <div class="stat-num">30%</div>
        <div class="stat-label">CPL Reduction</div>
      </div>
      <div class="stat-cell">
        <div class="stat-num">∞</div>
        <div class="stat-label">Creatives Shipped</div>
      </div>
    </div>
    <div class="hero-location">📍 Kochi, Kerala</div>
  </div>
</section>

<!-- ── 2. ABOUT ── -->
<section id="about">
  <div class="section-tag">About Me</div>
  <h2 class="section-title">The person behind<br>the <em>strategy</em></h2>
  <div class="about-grid">
    <div class="about-body reveal">
      <p>I am <strong>Akhil C A</strong>, a Social Media Manager based in Kochi with a deep passion for performance marketing and creative storytelling. My work lives at the intersection of data and design — where <em>numbers meet narrative</em>.</p>
      <p>Over 3+ years, I've served as the sole marketing resource at a multi-client agency, which means I've worn every hat — <strong>strategist, copywriter, designer, analyst, and automation engineer</strong> — simultaneously, for 10+ accounts at once.</p>
      <p>I don't just manage social media. I build audience relationships, reduce cost-per-lead through relentless A/B testing, and turn campaign data into decisions that actually move the needle.</p>
      <div class="divider"></div>
      <p style="font-size:0.8rem; color: var(--warm-gray); letter-spacing:0.05em;">Currently available for new opportunities &amp; freelance collaborations.</p>
    </div>
    <div class="about-highlights">
      <div class="highlight-item reveal reveal-delay-1">
        <div class="hi-icon">🎯</div>
        <div class="hi-title">Performance-First Mindset</div>
        <div class="hi-text">Every creative decision is backed by data. I track KPIs obsessively and optimise campaigns until the numbers tell a better story.</div>
      </div>
      <div class="highlight-item reveal reveal-delay-2">
        <div class="hi-icon">🎨</div>
        <div class="hi-title">End-to-End Creative</div>
        <div class="hi-text">From concept to pixel-perfect post — I design static, carousel, and video creatives using Photoshop, Illustrator, and Canva.</div>
      </div>
      <div class="highlight-item reveal reveal-delay-3">
        <div class="hi-icon">⚙️</div>
        <div class="hi-title">Automation &amp; Systems</div>
        <div class="hi-text">I build Zapier workflows, GTM configurations, and lead routing systems that reduce manual workload and improve data integrity.</div>
      </div>
    </div>
  </div>
</section>

<!-- ── 3. EXPERIENCE ── -->
<section id="experience">
  <div class="section-tag">Professional Journey</div>
  <h2 class="section-title">Where I've <em>worked</em></h2>
  <div class="timeline">

    <div class="timeline-item reveal">
      <div class="timeline-period">Oct 2025 – Feb 2026</div>
      <div class="timeline-role">Freelance Social Media Manager</div>
      <div class="timeline-company">Self-Employed — Remote, India</div>
      <ul class="timeline-bullets">
        <li>Delivered end-to-end social media management and paid social campaigns across solar, eco-product, and family entertainment verticals.</li>
        <li><strong style="color:rgba(245,240,232,0.85)">A3S Solar:</strong> Reduced cost-per-lead by 30% through iterative A/B testing of creatives and audience segments.</li>
        <li><strong style="color:rgba(245,240,232,0.85)">Ecoworm:</strong> Developed full content strategy alongside Facebook awareness and lead campaigns, managing creatives and reporting end-to-end.</li>
        <li><strong style="color:rgba(245,240,232,0.85)">Monkeybar Play Date Cafe:</strong> Managed organic content calendar and ran localised Meta Ads for summer workshops and seasonal events.</li>
      </ul>
    </div>

    <div class="timeline-item reveal reveal-delay-1">
      <div class="timeline-period">May 2023 – Jul 2025</div>
      <div class="timeline-role">Social Media Manager</div>
      <div class="timeline-company">ORIGONXT Solution Pvt Ltd — Kaloor, India</div>
      <ul class="timeline-bullets">
        <li>Sole marketing resource managing strategy, creative production, community engagement, and paid campaigns for 10+ simultaneous client accounts.</li>
        <li>Owned Facebook and Instagram strategy — creating and scheduling daily posts, stories, and reels while preserving each brand's distinct voice.</li>
        <li>Produced all organic and paid creatives using Photoshop, Illustrator, and Canva; ensured visual consistency across every account.</li>
        <li>Launched and optimised Meta Ads campaigns handling audience segmentation, A/B creative testing, budget management, and performance improvements.</li>
        <li>Monitored KPIs via Meta Ads Manager, GA4, and Microsoft Clarity; prepared monthly client-ready performance reports.</li>
        <li>Built Zapier automations for lead capture and CRM routing; implemented GTM tracking across client websites and landing pages.</li>
      </ul>
    </div>

    <div class="timeline-item reveal reveal-delay-2">
      <div class="timeline-period">Jul 2022 – Dec 2022</div>
      <div class="timeline-role">Social Media &amp; Digital Marketing Intern</div>
      <div class="timeline-company">SOFTERN Technologies — Kadavantra, India</div>
      <ul class="timeline-bullets">
        <li>Completed a 6-month structured training programme in social media marketing, paid social, SEO, and analytics.</li>
        <li>Practised content planning, Facebook Ads Manager, community management, and performance tracking using Google Analytics, Hootsuite, and Buffer.</li>
        <li>Progressed to independent client management within 6 months of graduating the programme.</li>
      </ul>
    </div>

  </div>
</section>

<!-- ── 4. CASE STUDIES ── -->
<section id="case-studies">
  <div class="section-tag">Work &amp; Results</div>
  <h2 class="section-title">Selected <em>campaigns</em></h2>
  <div class="cases-grid">

    <div class="case-card reveal">
      <div class="case-number">01</div>
      <div class="case-brand">A3S Solar</div>
      <div class="case-title">Meta Ads Lead Generation Campaign</div>
      <div class="case-body">Ran a targeted lead-gen campaign with iterative A/B testing across ad creatives and audience segments, significantly reducing acquisition costs.</div>
      <span class="case-metric">−30%</span>
      <span class="case-metric-label">Cost-Per-Lead Reduction</span>
    </div>

    <div class="case-card reveal reveal-delay-1">
      <div class="case-number">02</div>
      <div class="case-brand">Ecoworm</div>
      <div class="case-title">Full Content Strategy &amp; Paid Awareness</div>
      <div class="case-body">Developed brand-aligned content strategy for an eco-product company, layered with Facebook awareness and lead campaigns managed end-to-end.</div>
      <span class="case-metric">360°</span>
      <span class="case-metric-label">End-to-End Ownership</span>
    </div>

    <div class="case-card reveal reveal-delay-2">
      <div class="case-number">03</div>
      <div class="case-brand">Monkeybar Play Date Cafe</div>
      <div class="case-title">Localised Event Promotion Campaigns</div>
      <div class="case-body">Managed organic content and ran localised Meta Ads for summer workshops and seasonal events, targeting parents in specific Kochi localities.</div>
      <span class="case-metric">📍</span>
      <span class="case-metric-label">Hyper-Local Targeting</span>
    </div>

    <div class="case-card reveal reveal-delay-3">
      <div class="case-number">04</div>
      <div class="case-brand">ORIGONXT — Multi-Client</div>
      <div class="case-title">10+ Account Agency Management</div>
      <div class="case-body">Simultaneously managed social strategy, creative production, paid campaigns, and performance reporting for 10+ clients as the sole marketing resource.</div>
      <span class="case-metric">10+</span>
      <span class="case-metric-label">Active Accounts at Once</span>
    </div>

    <div class="case-card reveal reveal-delay-4">
      <div class="case-number">05</div>
      <div class="case-brand">Cross-Client</div>
      <div class="case-title">Zapier Lead Capture Automation</div>
      <div class="case-body">Built Zapier automations for lead capture and CRM routing across multiple client campaigns, reducing manual handoff time and improving data accuracy.</div>
      <span class="case-metric">⚙️</span>
      <span class="case-metric-label">Workflow Automation</span>
    </div>

    <div class="case-card reveal reveal-delay-5">
      <div class="case-number">06</div>
      <div class="case-brand">Cross-Client</div>
      <div class="case-title">GTM &amp; Analytics Implementation</div>
      <div class="case-body">Implemented Google Tag Manager tracking across client websites and campaign landing pages, enabling accurate conversion tracking and performance reporting.</div>
      <span class="case-metric">GA4</span>
      <span class="case-metric-label">Analytics Stack Built</span>
    </div>

  </div>
</section>

<!-- ── 5. SKILLS ── -->
<section id="skills">
  <div class="section-tag">Core Competencies</div>
  <h2 class="section-title">What I <em>do best</em></h2>
  <div class="skills-wrapper">
    <div class="skill-category reveal">
      <div class="skill-cat-title">Paid Social &amp; Ads</div>
      <div class="skill-bars">
        <div class="skill-bar-item">
          <div class="skill-bar-head"><span>Meta Ads Manager</span><span class="skill-bar-pct">95%</span></div>
          <div class="skill-bar-track"><div class="skill-bar-fill" style="width:95%"></div></div>
        </div>
        <div class="skill-bar-item">
          <div class="skill-bar-head"><span>Audience Targeting &amp; A/B Testing</span><span class="skill-bar-pct">90%</span></div>
          <div class="skill-bar-track"><div class="skill-bar-fill" style="width:90%"></div></div>
        </div>
        <div class="skill-bar-item">
          <div class="skill-bar-head"><span>Google Ads</span><span class="skill-bar-pct">75%</span></div>
          <div class="skill-bar-track"><div class="skill-bar-fill" style="width:75%"></div></div>
        </div>
        <div class="skill-bar-item">
          <div class="skill-bar-head"><span>Budget Management</span><span class="skill-bar-pct">88%</span></div>
          <div class="skill-bar-track"><div class="skill-bar-fill" style="width:88%"></div></div>
        </div>
      </div>
    </div>
    <div class="skill-category reveal reveal-delay-1">
      <div class="skill-cat-title">Content &amp; Creative</div>
      <div class="skill-bars">
        <div class="skill-bar-item">
          <div class="skill-bar-head"><span>Content Strategy</span><span class="skill-bar-pct">92%</span></div>
          <div class="skill-bar-track"><div class="skill-bar-fill" style="width:92%"></div></div>
        </div>
        <div class="skill-bar-item">
          <div class="skill-bar-head"><span>Adobe Photoshop &amp; Illustrator</span><span class="skill-bar-pct">85%</span></div>
          <div class="skill-bar-track"><div class="skill-bar-fill" style="width:85%"></div></div>
        </div>
        <div class="skill-bar-item">
          <div class="skill-bar-head"><span>Reels &amp; Short-Form Video</span><span class="skill-bar-pct">80%</span></div>
          <div class="skill-bar-track"><div class="skill-bar-fill" style="width:80%"></div></div>
        </div>
        <div class="skill-bar-item">
          <div class="skill-bar-head"><span>Community Management</span><span class="skill-bar-pct">88%</span></div>
          <div class="skill-bar-track"><div class="skill-bar-fill" style="width:88%"></div></div>
        </div>
      </div>
    </div>
    <div class="skill-category reveal reveal-delay-2">
      <div class="skill-cat-title">Analytics &amp; Reporting</div>
      <div class="skill-bars">
        <div class="skill-bar-item">
          <div class="skill-bar-head"><span>Google Analytics 4</span><span class="skill-bar-pct">85%</span></div>
          <div class="skill-bar-track"><div class="skill-bar-fill" style="width:85%"></div></div>
        </div>
        <div class="skill-bar-item">
          <div class="skill-bar-head"><span>Microsoft Clarity</span><span class="skill-bar-pct">78%</span></div>
          <div class="skill-bar-track"><div class="skill-bar-fill" style="width:78%"></div></div>
        </div>
        <div class="skill-bar-item">
          <div class="skill-bar-head"><span>SEMrush &amp; GSC</span><span class="skill-bar-pct">70%</span></div>
          <div class="skill-bar-track"><div class="skill-bar-fill" style="width:70%"></div></div>
        </div>
        <div class="skill-bar-item">
          <div class="skill-bar-head"><span>Client Performance Reporting</span><span class="skill-bar-pct">92%</span></div>
          <div class="skill-bar-track"><div class="skill-bar-fill" style="width:92%"></div></div>
        </div>
      </div>
    </div>
    <div class="skill-category reveal reveal-delay-3">
      <div class="skill-cat-title">Automation &amp; Tech</div>
      <div class="skill-bars">
        <div class="skill-bar-item">
          <div class="skill-bar-head"><span>Zapier Workflow Automation</span><span class="skill-bar-pct">82%</span></div>
          <div class="skill-bar-track"><div class="skill-bar-fill" style="width:82%"></div></div>
        </div>
        <div class="skill-bar-item">
          <div class="skill-bar-head"><span>Google Tag Manager</span><span class="skill-bar-pct">78%</span></div>
          <div class="skill-bar-track"><div class="skill-bar-fill" style="width:78%"></div></div>
        </div>
        <div class="skill-bar-item">
          <div class="skill-bar-head"><span>Hootsuite &amp; Buffer</span><span class="skill-bar-pct">85%</span></div>
          <div class="skill-bar-track"><div class="skill-bar-fill" style="width:85%"></div></div>
        </div>
        <div class="skill-bar-item">
          <div class="skill-bar-head"><span>CRM &amp; Lead Routing</span><span class="skill-bar-pct">75%</span></div>
          <div class="skill-bar-track"><div class="skill-bar-fill" style="width:75%"></div></div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ── 6. TOOLS ── -->
<section id="tools">
  <div class="section-tag">My Toolkit</div>
  <h2 class="section-title">Platforms &amp; <em>software</em></h2>
  <div class="tools-grid">
    <div class="tool-chip reveal"><span class="tool-icon">📣</span><span class="tool-name">Meta Ads Manager</span><span class="tool-cat-label">Paid Social</span></div>
    <div class="tool-chip reveal reveal-delay-1"><span class="tool-icon">🔍</span><span class="tool-name">Google Ads</span><span class="tool-cat-label">Paid Search</span></div>
    <div class="tool-chip reveal reveal-delay-2"><span class="tool-icon">📊</span><span class="tool-name">Google Analytics 4</span><span class="tool-cat-label">Analytics</span></div>
    <div class="tool-chip reveal reveal-delay-3"><span class="tool-icon">🏷️</span><span class="tool-name">Google Tag Manager</span><span class="tool-cat-label">Tracking</span></div>
    <div class="tool-chip reveal"><span class="tool-icon">🎨</span><span class="tool-name">Adobe Photoshop</span><span class="tool-cat-label">Design</span></div>
    <div class="tool-chip reveal reveal-delay-1"><span class="tool-icon">✏️</span><span class="tool-name">Adobe Illustrator</span><span class="tool-cat-label">Design</span></div>
    <div class="tool-chip reveal reveal-delay-2"><span class="tool-icon">🖼️</span><span class="tool-name">Canva</span><span class="tool-cat-label">Design</span></div>
    <div class="tool-chip reveal reveal-delay-3"><span class="tool-icon">🎬</span><span class="tool-name">Adobe Premiere Pro</span><span class="tool-cat-label">Video</span></div>
    <div class="tool-chip reveal"><span class="tool-icon">✂️</span><span class="tool-name">CapCut</span><span class="tool-cat-label">Video</span></div>
    <div class="tool-chip reveal reveal-delay-1"><span class="tool-icon">🔗</span><span class="tool-name">Zapier</span><span class="tool-cat-label">Automation</span></div>
    <div class="tool-chip reveal reveal-delay-2"><span class="tool-icon">📅</span><span class="tool-name">Hootsuite</span><span class="tool-cat-label">Scheduling</span></div>
    <div class="tool-chip reveal reveal-delay-3"><span class="tool-icon">📡</span><span class="tool-name">Buffer</span><span class="tool-cat-label">Scheduling</span></div>
    <div class="tool-chip reveal"><span class="tool-icon">🔎</span><span class="tool-name">SEMrush</span><span class="tool-cat-label">SEO</span></div>
    <div class="tool-chip reveal reveal-delay-1"><span class="tool-icon">🖱️</span><span class="tool-name">Microsoft Clarity</span><span class="tool-cat-label">Heatmaps</span></div>
    <div class="tool-chip reveal reveal-delay-2"><span class="tool-icon">📈</span><span class="tool-name">Google Search Console</span><span class="tool-cat-label">SEO</span></div>
    <div class="tool-chip reveal reveal-delay-3"><span class="tool-icon">🎞️</span><span class="tool-name">Wondershare Filmora</span><span class="tool-cat-label">Video</span></div>
  </div>
</section>

<!-- ── 7. CERTIFICATIONS ── -->
<section id="certifications">
  <div class="section-tag">Certifications</div>
  <h2 class="section-title">Credentials &amp; <em>learning</em></h2>
  <div class="certs-grid">
    <div class="cert-card reveal">
      <div class="cert-badge">🏅</div>
      <div class="cert-body">
        <div class="cert-issuer">Google Digital Garage</div>
        <div class="cert-name">Fundamentals of Digital Marketing</div>
        <div class="cert-desc">Covers SEO, SEM, analytics, social media marketing, content marketing, and email marketing fundamentals.</div>
      </div>
    </div>
    <div class="cert-card reveal reveal-delay-1">
      <div class="cert-badge">🎓</div>
      <div class="cert-body">
        <div class="cert-issuer">HubSpot Academy</div>
        <div class="cert-name">Digital Marketing Certification</div>
        <div class="cert-desc">Advanced certification covering inbound marketing, content strategy, social media, email, and paid advertising.</div>
      </div>
    </div>
  </div>
</section>

<!-- ── 8. EDUCATION ── -->
<section id="education">
  <div class="section-tag">Education</div>
  <h2 class="section-title">Academic <em>foundation</em></h2>
  <div class="edu-block reveal">
    <div>
      <div class="edu-year">2019<br>—<br>2022</div>
    </div>
    <div>
      <div class="edu-degree">Bachelor of Travel &amp; Tourism Management</div>
      <div class="edu-inst">Kerala, India</div>
      <div class="edu-note">
        A three-year undergraduate degree that built strong foundations in communication, client management, hospitality operations, and cross-cultural understanding — skills that directly translate to managing diverse brand voices and client relationships in the marketing industry.
      </div>
    </div>
  </div>
</section>

<!-- ── 9. CONTACT ── -->
<section id="contact">
  <div class="section-tag">Let's Connect</div>
  <h2 class="section-title">Ready to <em>collaborate</em></h2>
  <div class="contact-layout">
    <div>
      <p class="contact-intro">Whether you need a performance-obsessed social media manager, a creative campaign strategist, or someone to own your entire digital presence — I'd love to hear about your project.</p>
      <div class="contact-details">
        <div class="contact-item">
          <span class="contact-icon">📧</span>
          <div>
            <div class="contact-label">Email</div>
            <div class="contact-value"><a href="mailto:akhilcadm@gmail.com">akhilcadm@gmail.com</a></div>
          </div>
        </div>
        <div class="contact-item">
          <span class="contact-icon">📱</span>
          <div>
            <div class="contact-label">Phone / WhatsApp</div>
            <div class="contact-value"><a href="tel:+918089853390">+91 80898 53390</a></div>
          </div>
        </div>
        <div class="contact-item">
          <span class="contact-icon">📍</span>
          <div>
            <div class="contact-label">Location</div>
            <div class="contact-value">Kochi, Kerala, India</div>
          </div>
        </div>
      </div>
      <div class="contact-availability">
        <span class="avail-dot"></span>
        <span class="avail-text">Available for new roles &amp; freelance projects</span>
      </div>
    </div>

  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="footer-name">Akhil C A — Social Media Manager</div>
  <div style="display:flex; align-items:center; gap:0.6rem;">
    <span style="width:7px;height:7px;border-radius:50%;background:#6bcf7f;display:inline-block;animation:pulse 2s infinite;"></span>
    <span class="footer-note">Available for new roles</span>
  </div>
  <div class="footer-note">Kochi, India &nbsp;·&nbsp; 2025</div>
</footer>

<script>
  // Intersection Observer for reveal animations
  const revealEls = document.querySelectorAll('.reveal');
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(e => {
      if (e.isIntersecting) { e.target.classList.add('visible'); }
    });
  }, { threshold: 0.12, rootMargin: '0px 0px -40px 0px' });
  revealEls.forEach(el => observer.observe(el));

  // Nav background on scroll
  const nav = document.querySelector('nav');
  window.addEventListener('scroll', () => {
    if (window.scrollY > 60) {
      nav.style.boxShadow = '0 2px 30px rgba(0,0,0,0.08)';
    } else {
      nav.style.boxShadow = 'none';
    }
  });

  // Skill bar animations triggered on scroll
  const skillBars = document.querySelectorAll('.skill-bar-fill');
  const barObserver = new IntersectionObserver((entries) => {
    entries.forEach(e => {
      if (e.isIntersecting) {
        e.target.style.animationPlayState = 'running';
      }
    });
  }, { threshold: 0.5 });
  skillBars.forEach(bar => {
    bar.style.animationPlayState = 'paused';
    barObserver.observe(bar);
  });
</script>
</body>
</html>
