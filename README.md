[index.html](https://github.com/user-attachments/files/27443528/index.html)
# tb-hyponamiru
Teambuilding hyponamiru 2026
<!DOCTYPE html>
<html lang="cs">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Teambuilding hyponamiru — Branná, 16.–18. 6. 2026</title>
<meta name="description" content="Firemní teambuilding hyponamiru v apartmánech NoNe v Branné v Jeseníkách, 16.–18. června 2026.">

<!-- ============================================================
     OBSAH SE SNADNO UPRAVUJE — všechny texty jsou v HTML níže.
     Pokud chceš něco změnit (např. doplnit výlet), napiš mi a
     já ti to upravím.
============================================================ -->

<style>
  @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;900&family=Inter:wght@300;400;500;600;700&display=swap');

  :root {
    --green: #2d4a3e;
    --green-dark: #1f3329;
    --gold: #c9a87c;
    --cream: #fdfbf7;
    --sand: #f5f0e6;
    --ink: #1a1a1a;
    --muted: #6b6b6b;
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  html { scroll-behavior: smooth; }
  body {
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
    color: var(--ink);
    background: var(--cream);
    line-height: 1.6;
    -webkit-font-smoothing: antialiased;
  }

  img { max-width: 100%; display: block; }
  a { color: inherit; }

  /* ===================== NAVIGACE ===================== */
  .nav {
    position: sticky; top: 0;
    background: rgba(253,251,247,0.92);
    backdrop-filter: blur(12px);
    border-bottom: 1px solid #e8e2d6;
    z-index: 100;
    padding: 14px 32px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .nav .logo {
    display: flex;
    align-items: center;
    gap: 14px;
    text-decoration: none;
  }
  .nav .logo img {
    height: 30px;
    width: auto;
    display: block;
  }
  .nav .logo .badge-tb {
    font-family: 'Playfair Display', serif;
    font-weight: 700;
    font-size: 12px;
    letter-spacing: 2px;
    text-transform: uppercase;
    color: var(--gold);
    padding-left: 14px;
    border-left: 1px solid #d4cdb9;
  }
  @media (max-width: 720px) {
    .nav .logo img { height: 24px; }
    .nav .logo .badge-tb { display: none; }
  }
  .nav-links {
    display: flex;
    gap: 28px;
    list-style: none;
    font-size: 14px;
    font-weight: 500;
  }
  .nav-links a {
    text-decoration: none;
    color: var(--ink);
    transition: color 0.2s;
  }
  .nav-links a:hover { color: var(--green); }
  .nav-cta {
    padding: 8px 18px;
    background: var(--green);
    color: var(--cream) !important;
    border-radius: 999px;
    font-weight: 600;
    transition: background 0.2s;
  }
  .nav-cta:hover { background: var(--green-dark); }
  @media (max-width: 720px) {
    .nav { padding: 12px 16px; }
    .nav-links { display: none; }
  }

  /* ===================== HERO ===================== */
  .hero {
    position: relative;
    min-height: 92vh;
    background-image: url('https://noneapartmany.cz/wp-content/uploads/2023/08/dji_0099-enhanced-nr.jpg');
    background-size: cover;
    background-position: center;
    color: #fff;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 64px 24px;
    text-align: center;
  }
  .hero::after {
    content: ''; position: absolute; inset: 0;
    background: linear-gradient(180deg, rgba(0,0,0,0.25) 0%, rgba(0,0,0,0.55) 70%, rgba(0,0,0,0.85) 100%);
  }
  .hero-content { position: relative; z-index: 2; max-width: 900px; }
  .hero .badge {
    display: inline-block;
    padding: 8px 22px;
    background: rgba(255,255,255,0.12);
    backdrop-filter: blur(8px);
    border: 1px solid rgba(255,255,255,0.3);
    border-radius: 999px;
    font-size: 12px;
    letter-spacing: 3px;
    text-transform: uppercase;
    font-weight: 600;
    margin-bottom: 28px;
  }
  .hero h1 {
    font-family: 'Playfair Display', serif;
    font-weight: 900;
    font-size: clamp(48px, 8vw, 96px);
    line-height: 1.0;
    letter-spacing: -2px;
    margin-bottom: 24px;
    text-shadow: 0 4px 30px rgba(0,0,0,0.3);
  }
  .hero h1 em {
    font-style: italic;
    color: var(--gold);
    font-weight: 700;
  }
  .hero .lead {
    font-size: clamp(18px, 2vw, 22px);
    font-weight: 400;
    opacity: 0.95;
    max-width: 640px;
    margin: 0 auto 36px;
  }
  .hero-meta {
    display: flex;
    flex-wrap: wrap;
    gap: 32px;
    justify-content: center;
    margin-bottom: 36px;
  }
  .meta-item .label {
    font-size: 11px;
    letter-spacing: 2px;
    text-transform: uppercase;
    opacity: 0.7;
    margin-bottom: 4px;
  }
  .meta-item .value {
    font-family: 'Playfair Display', serif;
    font-size: 24px;
    font-weight: 700;
  }

  /* ===================== DEADLINE BANNER ===================== */
  .deadline-banner {
    background: var(--gold);
    color: var(--ink);
    padding: 22px 24px;
    text-align: center;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
    gap: 14px 28px;
  }
  .deadline-banner .icon {
    font-size: 22px;
  }
  .deadline-banner .text {
    font-size: 15px;
    font-weight: 500;
  }
  .deadline-banner strong {
    font-weight: 800;
  }
  .deadline-banner a {
    display: inline-block;
    padding: 10px 22px;
    background: var(--green);
    color: var(--cream);
    text-decoration: none;
    border-radius: 999px;
    font-weight: 700;
    font-size: 13px;
    letter-spacing: 0.5px;
    transition: background 0.2s;
  }
  .deadline-banner a:hover { background: var(--green-dark); }

  /* ===================== SEKCE ===================== */
  .section {
    padding: 96px 24px;
    max-width: 1100px;
    margin: 0 auto;
  }
  .section.dark { background: var(--sand); max-width: none; padding-left: 24px; padding-right: 24px; }
  .section.dark .section-inner { max-width: 1100px; margin: 0 auto; }

  .eyebrow {
    font-size: 11px;
    letter-spacing: 3px;
    text-transform: uppercase;
    color: var(--gold);
    font-weight: 600;
    margin-bottom: 14px;
  }
  .section-title {
    font-family: 'Playfair Display', serif;
    font-size: clamp(36px, 5vw, 56px);
    font-weight: 900;
    color: var(--green);
    line-height: 1.05;
    margin-bottom: 24px;
    letter-spacing: -1px;
  }
  .section-lead {
    font-size: 18px;
    color: var(--muted);
    max-width: 720px;
    margin-bottom: 56px;
  }

  /* ===================== PROGRAM ===================== */
  .day {
    margin-bottom: 48px;
    padding-bottom: 48px;
    border-bottom: 1px solid #e8e2d6;
  }
  .day:last-child { border-bottom: none; }
  .day-header {
    display: flex;
    align-items: baseline;
    gap: 18px;
    flex-wrap: wrap;
    margin-bottom: 24px;
  }
  .day-date {
    font-family: 'Playfair Display', serif;
    font-size: 32px;
    font-weight: 700;
    color: var(--green);
  }
  .day-label {
    font-size: 12px;
    text-transform: uppercase;
    letter-spacing: 2px;
    color: var(--gold);
    font-weight: 600;
    padding: 4px 14px;
    border: 1px solid var(--gold);
    border-radius: 999px;
  }
  .timeline {
    display: grid;
    grid-template-columns: 140px 1fr;
    gap: 12px 28px;
  }
  .time {
    font-weight: 700;
    color: var(--green);
    font-size: 15px;
    padding: 10px 0;
    font-variant-numeric: tabular-nums;
  }
  .activity {
    padding: 10px 0;
    font-size: 16px;
  }
  .activity strong { display: block; color: var(--ink); }
  .activity .note {
    font-size: 13px;
    color: var(--muted);
    font-style: italic;
    margin-top: 2px;
  }
  .day-note {
    margin-top: 18px;
    padding: 10px 14px;
    background: #fffbf0;
    border-left: 3px solid var(--gold);
    color: var(--muted);
    font-size: 13px;
    border-radius: 4px;
  }
  .variant-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 18px;
    margin-top: 24px;
  }
  .variant {
    background: #fff;
    border: 1px solid #e8e2d6;
    border-radius: 8px;
    padding: 24px;
    position: relative;
  }
  .variant-tag {
    display: inline-block;
    padding: 4px 12px;
    background: var(--green);
    color: var(--cream);
    font-size: 10px;
    letter-spacing: 2px;
    text-transform: uppercase;
    font-weight: 700;
    border-radius: 999px;
    margin-bottom: 12px;
  }
  .variant h4 {
    font-family: 'Playfair Display', serif;
    font-size: 24px;
    color: var(--green);
    margin-bottom: 10px;
  }
  .variant-desc {
    font-size: 14px;
    color: var(--ink);
    margin-bottom: 14px;
    line-height: 1.55;
  }
  .variant-meta {
    list-style: none;
    padding: 0;
    margin: 0;
    border-top: 1px solid #e8e2d6;
    padding-top: 14px;
  }
  .variant-meta li {
    font-size: 13px;
    color: var(--muted);
    padding: 4px 0;
  }
  .variant-meta li strong {
    color: var(--ink);
    font-weight: 600;
  }
  @media (max-width: 600px) {
    .timeline { grid-template-columns: 1fr; gap: 0; }
    .time { padding-bottom: 0; }
    .activity { padding-top: 4px; padding-bottom: 16px; border-bottom: 1px dashed #e8e2d6; }
  }

  /* ===================== UBYTOVÁNÍ INFO ===================== */
  .feat-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 18px;
    margin-top: 32px;
  }
  .feat {
    padding: 24px;
    background: #fff;
    border: 1px solid #e8e2d6;
    border-radius: 8px;
  }
  .feat-icon {
    font-size: 24px;
    margin-bottom: 10px;
  }
  .feat-title {
    font-weight: 700;
    color: var(--green);
    margin-bottom: 6px;
  }
  .feat-desc { font-size: 14px; color: var(--muted); }

  /* ===================== GALERIE ===================== */
  .gallery {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 12px;
  }
  .gallery .photo {
    aspect-ratio: 4/3;
    background-size: cover;
    background-position: center;
    background-color: #d8cfbf;
    position: relative;
    overflow: hidden;
    border-radius: 6px;
    transition: transform 0.4s;
  }
  .gallery .photo:hover { transform: scale(1.02); }
  .gallery .photo.tall { grid-row: span 2; aspect-ratio: 4/6.2; }
  .gallery .caption {
    position: absolute;
    bottom: 0; left: 0; right: 0;
    padding: 14px 16px;
    background: linear-gradient(0deg, rgba(0,0,0,0.78) 0%, transparent 100%);
    color: #fff;
    font-size: 13px;
    font-weight: 600;
    letter-spacing: 0.5px;
  }
  @media (max-width: 720px) {
    .gallery { grid-template-columns: repeat(2, 1fr); }
    .gallery .photo.tall { grid-row: auto; aspect-ratio: 4/3; }
  }

  /* ===================== MAPA ===================== */
  .map-wrap {
    margin-top: 32px;
    border-radius: 8px;
    overflow: hidden;
    border: 1px solid #e8e2d6;
    background: #fff;
  }
  .map-illustration {
    display: block;
    width: 100%;
    height: auto;
  }
  .map-cta {
    display: block;
    text-align: center;
    padding: 16px;
    background: var(--green);
    color: var(--cream) !important;
    text-decoration: none;
    font-weight: 600;
    font-size: 15px;
    letter-spacing: 0.3px;
    transition: background 0.2s;
  }
  .map-cta:hover { background: var(--green-dark); }
  .travel {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 20px;
    margin-top: 28px;
  }
  .travel-card {
    padding: 24px;
    background: #fff;
    border: 1px solid #e8e2d6;
    border-radius: 8px;
  }
  .travel-card h4 {
    color: var(--green);
    margin-bottom: 8px;
    font-size: 16px;
  }
  .travel-card p { font-size: 14px; color: var(--muted); }

  /* ===================== CTA ===================== */
  .cta-section {
    background: var(--green);
    color: var(--cream);
    text-align: center;
    padding: 96px 24px;
  }
  .cta-section h2 {
    font-family: 'Playfair Display', serif;
    font-size: clamp(36px, 5vw, 56px);
    font-weight: 900;
    margin-bottom: 16px;
  }
  .cta-section p {
    font-size: 18px;
    opacity: 0.85;
    max-width: 600px;
    margin: 0 auto 32px;
  }
  .btn {
    display: inline-block;
    padding: 16px 36px;
    background: var(--gold);
    color: var(--ink);
    text-decoration: none;
    border-radius: 999px;
    font-weight: 700;
    font-size: 15px;
    letter-spacing: 0.5px;
    transition: transform 0.2s, box-shadow 0.2s;
  }
  .btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 12px 30px rgba(201,168,124,0.4);
  }
  .btn-secondary {
    background: transparent;
    border: 1.5px solid var(--cream);
    color: var(--cream);
    margin-left: 12px;
  }
  .deadline {
    font-size: 13px;
    opacity: 0.7;
    margin-top: 18px;
    letter-spacing: 0.5px;
  }

  /* ===================== TLAČÍTKO FORMULÁŘ ===================== */
  .btn-form {
    margin-top: 8px;
    padding: 18px 40px;
    font-size: 16px;
  }
  .form-note {
    margin-top: 18px;
    font-size: 13px;
    color: rgba(253,251,247,0.7);
    letter-spacing: 0.3px;
  }
  .link-card {
    max-width: 640px;
    margin: 32px auto 0;
    padding: 32px;
    background: rgba(253,251,247,0.08);
    border: 1px solid rgba(253,251,247,0.18);
    border-radius: 12px;
    text-align: center;
  }
  .link-card-icon {
    font-size: 36px;
    margin-bottom: 14px;
  }
  .link-card-label {
    font-size: 13px;
    letter-spacing: 1px;
    color: var(--gold);
    margin-bottom: 12px;
    font-weight: 600;
  }
  .link-card-url {
    display: block;
    background: rgba(0,0,0,0.25);
    color: var(--cream);
    padding: 14px 18px;
    border-radius: 6px;
    font-family: ui-monospace, SFMono-Regular, Menlo, monospace;
    font-size: 14px;
    word-break: break-all;
    user-select: all;
    margin-bottom: 18px;
    border: 1px dashed rgba(253,251,247,0.25);
  }
  .map-url {
    margin-top: 18px;
    padding: 16px 20px;
    background: var(--sand);
    border-radius: 6px;
    font-size: 14px;
    color: var(--ink);
    text-align: center;
  }
  .map-url strong {
    display: block;
    margin-bottom: 6px;
    color: var(--green);
    font-size: 12px;
    letter-spacing: 1px;
    text-transform: uppercase;
  }
  .map-url code {
    font-family: ui-monospace, SFMono-Regular, Menlo, monospace;
    color: var(--green);
    word-break: break-all;
    user-select: all;
  }

  /* ===================== FAQ ===================== */
  .faq-item {
    border-bottom: 1px solid #e8e2d6;
    padding: 20px 0;
  }
  .faq-q {
    font-weight: 600;
    color: var(--green);
    cursor: pointer;
    list-style: none;
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-size: 17px;
  }
  .faq-q::after {
    content: '+';
    font-size: 24px;
    font-weight: 300;
    transition: transform 0.2s;
  }
  details[open] .faq-q::after { transform: rotate(45deg); }
  .faq-a {
    margin-top: 12px;
    color: var(--muted);
    font-size: 15px;
    line-height: 1.7;
  }

  /* ===================== AKTUALITY ===================== */
  .news {
    background: #fffbf0;
    border-left: 4px solid var(--gold);
    padding: 20px 24px;
    border-radius: 4px;
    margin-bottom: 28px;
  }
  .news-date {
    font-size: 11px;
    letter-spacing: 2px;
    text-transform: uppercase;
    color: var(--gold);
    font-weight: 700;
    margin-bottom: 4px;
  }
  .news strong { color: var(--green); }

  /* ===================== FOOTER ===================== */
  .footer {
    background: var(--green-dark);
    color: rgba(253,251,247,0.7);
    padding: 56px 24px 32px;
    text-align: center;
    font-size: 14px;
  }
  .footer .footer-logo {
    margin-bottom: 18px;
  }
  .footer .footer-logo img {
    height: 36px;
    width: auto;
    display: inline-block;
  }
  .footer-meta {
    margin-top: 24px;
    font-size: 12px;
    opacity: 0.6;
    letter-spacing: 0.5px;
  }
  .footer a {
    color: var(--gold);
    text-decoration: none;
  }

</style>
</head>
<body>

<!-- ===================== NAVIGACE ===================== -->
<nav class="nav">
  <a href="#top" class="logo">
    <img src="data:image/png;base64,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" alt="hyponamiru">
    <span class="badge-tb">Teambuilding 2026</span>
  </a>
  <ul class="nav-links">
    <li><a href="#program">Program</a></li>
    <li><a href="#misto">Místo</a></li>
    <li><a href="#galerie">Galerie</a></li>
    <li><a href="#doprava">Doprava</a></li>
    <li><a href="#faq">FAQ</a></li>
  </ul>
  <a href="#registrace" class="nav-cta">Registrace</a>
</nav>

<!-- ===================== HERO ===================== -->
<header class="hero" id="top">
  <div class="hero-content">
    <span class="badge">Teambuilding · hyponamiru</span>
    <h1>Tři dny v <em>Jeseníkách</em></h1>
    <p class="lead">
      Společný teambuilding hyponamiru v apartmánech NoNe v Branné.
      Příroda, sauna, vířivka, výlety a parta — všechno na jednom místě.
    </p>
    <div class="hero-meta">
      <div class="meta-item">
        <div class="label">Termín</div>
        <div class="value">16. – 18. 6. 2026</div>
      </div>
      <div class="meta-item">
        <div class="label">Místo</div>
        <div class="value">Branná, Jeseníky</div>
      </div>
      <div class="meta-item">
        <div class="label">Příjezd / Odjezd</div>
        <div class="value">11:00 / 10:00</div>
      </div>
    </div>
    <a href="#registrace" class="btn">Registruj se</a>
  </div>
</header>


<!-- ===================== DEADLINE BANNER ===================== -->
<div class="deadline-banner">
  <span class="icon">📝</span>
  <span class="text">Prosíme, vyplň <strong>registrační dotazník do 15. 5. 2026</strong>, ať můžeme vše připravit.</span>
  <a href="#registrace">Vyplnit dotazník</a>
</div>

<!-- ===================== PROGRAM ===================== -->
<section class="section dark" id="program">
  <div class="section-inner">
    <div class="eyebrow">Program</div>
    <h2 class="section-title">Tři dny, jedno místo,<br>spousta zážitků</h2>
    <p class="section-lead">
      Detailní program postupně doplníme — výlety a aktivity ladíme podle počasí a vašich preferencí z dotazníku.
    </p>

    <!-- DEN 1 -->
    <div class="day">
      <div class="day-header">
        <span class="day-date">Úterý 16. 6.</span>
        <span class="day-label">Den 1 · Příjezd & Branná</span>
      </div>
      <div class="timeline">
        <div class="time">11:00</div>
        <div class="activity">
          <strong>Příjezd na místo</strong>
          <div class="note">Ubytování v apartmánech, uvítání</div>
        </div>

        <div class="time">12:30</div>
        <div class="activity">
          <strong>Procházka do Branné — Minipivovar Kolštejn</strong>
          <div class="note">Společný oběd a pití v <a href="https://kolstejn.cz/minipivovar/" target="_top" style="color: var(--green); text-decoration: underline;">minipivovaru Kolštejn</a></div>
        </div>

        <div class="time">15:30</div>
        <div class="activity">
          <strong>Prohlídka zámku Kolštejn</strong>
          <div class="note">Komentovaná prohlídka jedné z dominant Branné</div>
        </div>

        <div class="time">poté</div>
        <div class="activity">
          <strong>Procházka zpět na ubytování</strong>
        </div>

        <div class="time">od 18:00</div>
        <div class="activity">
          <strong>Grilování u ohně</strong>
          <div class="note">Večerní občerstvení & posezení</div>
        </div>

        <div class="time">celý večer</div>
        <div class="activity">
          <strong>Volný program — k dispozici</strong>
          <div class="note">🔥 oheň · 🛋️ společenská místnost · 🧖 sauna · ♨️ vířivka · 🏓 ping pong</div>
        </div>
      </div>
      <div class="day-note">
        <em>Program se může v závislosti na okolnostech ještě upravit.</em>
      </div>
    </div>

    <!-- DEN 2 -->
    <div class="day">
      <div class="day-header">
        <span class="day-date">Středa 17. 6.</span>
        <span class="day-label">Den 2 · Společný výlet</span>
      </div>
      <div class="timeline">
        <div class="time">8:00 – 10:00</div>
        <div class="activity"><strong>Snídaně</strong></div>

        <div class="time">10:00</div>
        <div class="activity">
          <strong>Vyrážíme na společný výlet</strong>
          <div class="note">Aktuálně zvažujeme dvě varianty (viz níže) — finální výběr upřesníme</div>
        </div>

        <div class="time">cca 19:00</div>
        <div class="activity"><strong>Návrat na místo</strong></div>

        <div class="time">od 19:00</div>
        <div class="activity">
          <strong>Večerní zábava u ohně</strong>
          <div class="note">Občerstvení & posezení pod hvězdami</div>
        </div>

        <div class="time">celý večer</div>
        <div class="activity">
          <strong>Volný program — k dispozici</strong>
          <div class="note">🔥 oheň · 🛋️ společenská místnost · 🧖 sauna · ♨️ vířivka · 🏓 ping pong</div>
        </div>
      </div>

      <!-- Dvě varianty výletu -->
      <div class="variant-grid">
        <div class="variant">
          <div class="variant-tag">Varianta A</div>
          <h4>🥾 Šerák pěšky</h4>
          <p class="variant-desc">
            Klasický společný výšlap z <strong>Ramzové</strong> na vrchol <strong>Šerák</strong> (1 351 m n. m.).
            Krásné výhledy, lesní cesty, zastávka na Jiřího chatě.
          </p>
          <ul class="variant-meta">
            <li><strong>Trvání:</strong> celý den, cca 5–6 h v pohybu</li>
            <li><strong>Náročnost:</strong> středně náročné, cca 12 km</li>
            <li><strong>Co s sebou:</strong> turistická obuv, voda, svačina</li>
            <li><strong>Cena:</strong> zdarma (případně lanovka Ramzová)</li>
          </ul>
        </div>

        <div class="variant">
          <div class="variant-tag">Varianta B</div>
          <h4>🎢 Dolní Morava</h4>
          <p class="variant-desc">
            Resort s mnoha atrakcemi pro každého — <strong>Stezka v oblacích</strong>, Mamutíkův vodní park,
            <strong>bobová dráha</strong>, lanový park, sedačka na Slamník.
          </p>
          <ul class="variant-meta">
            <li><strong>Trvání:</strong> celý den, atrakce dle výběru</li>
            <li><strong>Náročnost:</strong> nízká, lze přizpůsobit každému</li>
            <li><strong>Co s sebou:</strong> sportovní oděv, plavky (vodní park)</li>
            <li><strong>Cena:</strong> dle výběru atrakcí (vstupy)</li>
          </ul>
        </div>
      </div>

      <div class="day-note">
        <em>Finální výběr výletu upřesníme později podle počasí a preferencí účastníků z dotazníku.</em>
      </div>
    </div>

    <!-- DEN 3 -->
    <div class="day">
      <div class="day-header">
        <span class="day-date">Čtvrtek 18. 6.</span>
        <span class="day-label">Den 3 · Odjezd</span>
      </div>
      <div class="timeline">
        <div class="time">8:00 – 10:00</div>
        <div class="activity"><strong>Snídaně</strong></div>

        <div class="time">10:00</div>
        <div class="activity">
          <strong>Check-out</strong>
          <div class="note">Odjezd domů</div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ===================== MÍSTO / UBYTOVÁNÍ ===================== -->
<section class="section" id="misto">
  <div class="eyebrow">Místo konání</div>
  <h2 class="section-title">Apartmány NoNe<br>v srdci Jeseníků</h2>
  <p class="section-lead">
    Stylové ubytování ve skalách s výhledem na obec Branná. Až 46 lůžek v 10 apartmánech a samostatném domečku, kompletní wellness zázemí, společenské prostory a venkovní areál.
    <br><br>
    <a href="https://noneapartmany.cz" target="_top" style="color: var(--green); font-weight: 600;">noneapartmany.cz →</a>
  </p>

  <div class="feat-grid">
    <div class="feat">
      <div class="feat-icon">🏡</div>
      <div class="feat-title">Apartmány</div>
      <div class="feat-desc">Až 46 lůžek, masivní nábytek, plně vybavené kuchyně, krbová kamna, Wi-Fi, TV</div>
    </div>
    <div class="feat">
      <div class="feat-icon">🧖</div>
      <div class="feat-title">Sauna</div>
      <div class="feat-desc">Finská sauna, sprchový kout, odpočívárna</div>
    </div>
    <div class="feat">
      <div class="feat-icon">♨️</div>
      <div class="feat-title">Venkovní vířivka</div>
      <div class="feat-desc">Hot Tub pod širým nebem s výhledem do přírody</div>
    </div>
    <div class="feat">
      <div class="feat-icon">🔥</div>
      <div class="feat-title">Ohniště</div>
      <div class="feat-desc">Venkovní ohniště pro večerní opékání a posezení</div>
    </div>
    <div class="feat">
      <div class="feat-icon">🌿</div>
      <div class="feat-title">Areál</div>
      <div class="feat-desc">Přírodní jezírko, zahrada, hřiště, ping-pong, vinný sklípek</div>
    </div>
    <div class="feat">
      <div class="feat-icon">🛋️</div>
      <div class="feat-title">Společenská místnost</div>
      <div class="feat-desc">Krbová kamna, prostor pro celou skupinu</div>
    </div>
  </div>
</section>

<!-- ===================== GALERIE ===================== -->
<section class="section dark" id="galerie">
  <div class="section-inner">
    <div class="eyebrow">Galerie</div>
    <h2 class="section-title">Co nás čeká</h2>

    <div class="gallery">
      <div class="photo tall" style="background-image:url('https://noneapartmany.cz/wp-content/uploads/2023/08/dji_0113-enhanced-nr.jpg')">
        <div class="caption">Areál z dronu</div>
      </div>
      <div class="photo" style="background-image:url('https://noneapartmany.cz/wp-content/uploads/2022/08/untitled-78-of-201.jpg')">
        <div class="caption">Apartmány</div>
      </div>
      <div class="photo" style="background-image:url('https://noneapartmany.cz/wp-content/uploads/2022/10/untitled-9-of-201.jpg')">
        <div class="caption">Společenské prostory</div>
      </div>
      <div class="photo" style="background-image:url('https://noneapartmany.cz/wp-content/uploads/2023/02/dsc01281.jpg')">
        <div class="caption">Sauna</div>
      </div>
      <div class="photo" style="background-image:url('https://noneapartmany.cz/wp-content/uploads/2022/08/koupaci-sud-3.jpg')">
        <div class="caption">Vířivka</div>
      </div>
      <div class="photo" style="background-image:url('https://noneapartmany.cz/wp-content/uploads/2022/08/ohniste-2.jpg')">
        <div class="caption">Ohniště</div>
      </div>
      <div class="photo" style="background-image:url('https://noneapartmany.cz/wp-content/uploads/2022/08/jezirko-2.jpg')">
        <div class="caption">Jezírko</div>
      </div>
      <div class="photo" style="background-image:url('https://noneapartmany.cz/wp-content/uploads/2023/08/dsc09340.jpg')">
        <div class="caption">Příroda</div>
      </div>
    </div>
  </div>
</section>

<!-- ===================== DOPRAVA / MAPA ===================== -->
<section class="section" id="doprava">
  <div class="eyebrow">Doprava & Mapa</div>
  <h2 class="section-title">Jak se k nám dostaneš</h2>
  <p class="section-lead">
    Branná leží v Jeseníkách, kousek od Šumperka. Adresa: <strong>Branná 209, 788 25 Branná</strong>.
  </p>

  <div class="map-wrap">
    <svg viewBox="0 0 800 360" xmlns="http://www.w3.org/2000/svg" class="map-illustration" preserveAspectRatio="xMidYMid slice">
      <!-- Pozadí: nebe + hory + údolí -->
      <defs>
        <linearGradient id="skyGrad" x1="0" y1="0" x2="0" y2="1">
          <stop offset="0%" stop-color="#e8f0e6"/>
          <stop offset="100%" stop-color="#d4e0cf"/>
        </linearGradient>
        <linearGradient id="hillGrad1" x1="0" y1="0" x2="0" y2="1">
          <stop offset="0%" stop-color="#7a9a78"/>
          <stop offset="100%" stop-color="#5d7d5b"/>
        </linearGradient>
        <linearGradient id="hillGrad2" x1="0" y1="0" x2="0" y2="1">
          <stop offset="0%" stop-color="#94b08e"/>
          <stop offset="100%" stop-color="#6f8e6b"/>
        </linearGradient>
        <linearGradient id="valleyGrad" x1="0" y1="0" x2="0" y2="1">
          <stop offset="0%" stop-color="#a9c1a1"/>
          <stop offset="100%" stop-color="#85a07c"/>
        </linearGradient>
      </defs>

      <rect width="800" height="360" fill="url(#skyGrad)"/>

      <!-- Vzdálené hory -->
      <path d="M0,180 L60,140 L130,165 L200,120 L290,155 L370,110 L450,150 L520,125 L600,160 L690,130 L800,170 L800,360 L0,360 Z" fill="#9bb094" opacity="0.55"/>

      <!-- Střední hory -->
      <path d="M0,220 L80,180 L160,210 L240,170 L320,205 L410,165 L490,200 L570,175 L660,205 L740,180 L800,210 L800,360 L0,360 Z" fill="url(#hillGrad2)"/>

      <!-- Lesy v popředí -->
      <path d="M0,260 L60,240 L120,255 L180,235 L240,260 L300,240 L360,255 L420,230 L480,260 L540,240 L600,255 L660,235 L720,260 L800,245 L800,360 L0,360 Z" fill="url(#hillGrad1)"/>

      <!-- Údolí -->
      <path d="M0,310 L800,290 L800,360 L0,360 Z" fill="url(#valleyGrad)"/>

      <!-- Řeka -->
      <path d="M0,335 Q200,328 380,332 T800,325" stroke="#8db8d4" stroke-width="3" fill="none" opacity="0.7"/>

      <!-- Stromky -->
      <g fill="#3d5b3a">
        <circle cx="80" cy="278" r="6"/>
        <circle cx="105" cy="285" r="5"/>
        <circle cx="630" cy="282" r="6"/>
        <circle cx="660" cy="288" r="5"/>
        <circle cx="700" cy="280" r="7"/>
      </g>

      <!-- Domečky obce Branná -->
      <g>
        <rect x="290" y="295" width="22" height="18" fill="#d4a574"/>
        <polygon points="288,295 301,283 314,295" fill="#8b4513"/>
        <rect x="320" y="298" width="20" height="15" fill="#e8c8a0"/>
        <polygon points="318,298 330,287 342,298" fill="#a0522d"/>
        <rect x="350" y="296" width="18" height="17" fill="#d4a574"/>
        <polygon points="348,296 359,285 370,296" fill="#8b4513"/>
        <rect x="380" y="299" width="16" height="14" fill="#e8c8a0"/>
        <polygon points="378,299 388,289 398,299" fill="#a0522d"/>
      </g>

      <!-- Označení Branná -->
      <text x="335" y="333" text-anchor="middle" font-family="'Inter', sans-serif" font-size="11" font-weight="600" fill="#3a3a3a" letter-spacing="2">BRANNÁ</text>

      <!-- Pin uprostřed -->
      <g transform="translate(400,150)">
        <!-- Pulzující kruh -->
        <circle cx="0" cy="115" r="20" fill="#c9a87c" opacity="0.25"/>
        <circle cx="0" cy="115" r="12" fill="#c9a87c" opacity="0.4"/>
        <!-- Pin shape -->
        <path d="M0,40 C-22,40 -38,58 -38,80 C-38,108 0,150 0,150 C0,150 38,108 38,80 C38,58 22,40 0,40 Z" fill="#2d4a3e" stroke="#1f3329" stroke-width="2"/>
        <circle cx="0" cy="80" r="14" fill="#fdfbf7"/>
        <text x="0" y="86" text-anchor="middle" font-family="'Inter', sans-serif" font-size="16" font-weight="700" fill="#2d4a3e">N</text>
      </g>

      <!-- Popisek -->
      <g>
        <rect x="305" y="35" width="190" height="48" rx="6" fill="#fdfbf7" stroke="#2d4a3e" stroke-width="1.5"/>
        <text x="400" y="55" text-anchor="middle" font-family="'Playfair Display', serif" font-size="15" font-weight="700" fill="#2d4a3e">Apartmány NoNe</text>
        <text x="400" y="73" text-anchor="middle" font-family="'Inter', sans-serif" font-size="11" fill="#6b6b6b">Branná 209, 788 25</text>
      </g>

      <!-- Spojovací linka popisek-pin -->
      <line x1="400" y1="83" x2="400" y2="190" stroke="#2d4a3e" stroke-width="1.5" stroke-dasharray="3,3" opacity="0.5"/>
    </svg>
    <a class="map-cta" href="https://maps.google.com/?q=Apartm%C3%A1ny+NoNe+Brann%C3%A1+209" target="_top" rel="noopener">
      📍 Otevřít v Google Maps
    </a>
  </div>
  <div class="map-url">
    <strong>Odkaz na mapu:</strong>
    <code>https://maps.google.com/?q=Apartmány+NoNe+Branná+209</code>
  </div>

  <div class="travel">
    <div class="travel-card">
      <h4>🚗 Autem</h4>
      <p>
        Z Prahy ~3,5 hod, z Brna ~2 hod. Parkování přímo u apartmánů.
        Pokud nabízíš spolujízdu nebo se chceš svézt, vyplň to v dotazníku.
      </p>
    </div>
    <div class="travel-card">
      <h4>🚆 Vlakem</h4>
      <p>
        Nejbližší zastávka: <strong>Branná</strong> (přestup v Hanušovicích nebo Šumperku).
        Z nádraží je to k apartmánům cca 5 min pěšky.
      </p>
    </div>
    <div class="travel-card">
      <h4>📍 Adresa</h4>
      <p>
        Branná 209, 788 25 Branná<br>
        <a href="https://maps.google.com/?q=Apartm%C3%A1ny+NoNe+Brann%C3%A1+209" target="_top" style="color: var(--green); font-weight: 600;">Otevřít v Google Maps →</a>
      </p>
    </div>
  </div>
</section>

<!-- ===================== REGISTRACE — VESTAVĚNÝ GOOGLE FORM ===================== -->
<section class="cta-section" id="registrace">
  <div class="eyebrow" style="color: var(--gold);">Registrace</div>
  <h2>Dáváš vědět, jestli jedeš</h2>
  <p>
    Vyplň krátký dotazník přímo zde — stravovací preference, zájem o saunu, vířivku a večerní oheň.
    Zabere ti to 2 minuty a pomůže nám připravit všechno na míru.
  </p>

  <div class="deadline">Prosíme o vyplnění do <strong>15. 5. 2026</strong></div>

  <div class="link-card">
    <div class="link-card-icon">📝</div>
    <div class="link-card-label">Odkaz na dotazník — zkopíruj a otevři v prohlížeči:</div>
    <div class="link-card-url">https://forms.cloud.microsoft/e/xVC8i3eN88</div>
    <a href="https://forms.cloud.microsoft/e/xVC8i3eN88" target="_top" rel="noopener" class="btn btn-form">
      Vyplnit dotazník
    </a>
  </div>
  <p class="form-note">Otevře se Microsoft Forms. Pro vyplnění se přihlas svým hyponamiru účtem.</p>
</section>

<!-- ===================== FAQ ===================== -->
<section class="section" id="faq">
  <div class="eyebrow">Časté otázky</div>
  <h2 class="section-title">FAQ</h2>

  <details class="faq-item">
    <summary class="faq-q">Co si mám vzít s sebou?</summary>
    <div class="faq-a">
      Pohodlné oblečení a obuv na výlety, plavky (sauna a vířivka), případně teplejší vrstvu na večery v horách.
      Ručníky a ložní prádlo jsou v apartmánech k dispozici.
    </div>
  </details>

  <details class="faq-item">
    <summary class="faq-q">Jak je to s jídlem?</summary>
    <div class="faq-a">
      Snídaně, obědy a večeře zajistíme společně. V dotazníku, prosím, uveď stravovací preference (s masem / bez masa / vegan / bezlepkové) a případné alergie.
    </div>
  </details>

  <details class="faq-item">
    <summary class="faq-q">Co když přijedu později nebo odjedu dříve?</summary>
    <div class="faq-a">
      Žádný problém. Uveď to prosím v dotazníku, ať s tebou počítáme správně u jídla a výletů.
    </div>
  </details>

  <details class="faq-item">
    <summary class="faq-q">Je v apartmánech Wi-Fi?</summary>
    <div class="faq-a">
      Ano, ve všech apartmánech je Wi-Fi a TV. Ale doporučujeme spíš odpočívat 🙂
    </div>
  </details>
</section>

<!-- ===================== FOOTER ===================== -->
<footer class="footer">
  <div class="footer-logo">
    <img src="data:image/png;base64,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" alt="hyponamiru">
  </div>
  <div>Teambuilding · 16.–18. června 2026 · Branná, Jeseníky</div>
  <div style="margin-top: 16px;">
    Apartmány NoNe · <a href="https://noneapartmany.cz" target="_top">noneapartmany.cz</a>
  </div>
  <div class="footer-meta">
    Otázky? Napiš pořadatelům · Web aktualizován 6. 5. 2026
  </div>
</footer>


</body>
</html>
