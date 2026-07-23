<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>OBRA — Estudio de Arquitectura</title>
<meta name="description" content="OBRA es un estudio de arquitectura enfocado en diseño residencial, planificación y soluciones a medida.">

<!-- Favicon (usa la marca del sitio, sin archivos extra que subir) -->
<link rel="icon" type="image/svg+xml" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 40 40'%3E%3Crect width='40' height='40' fill='%23ECE9E1'/%3E%3Cpath d='M4 32 L20 8 L36 32' fill='none' stroke='%231B1D1E' stroke-width='3' stroke-linejoin='round' stroke-linecap='round'/%3E%3Cline x1='10' y1='32' x2='10' y2='22' stroke='%231B1D1E' stroke-width='3'/%3E%3Cline x1='30' y1='32' x2='30' y2='22' stroke='%231B1D1E' stroke-width='3'/%3E%3C/svg%3E">
<link rel="alternate icon" href="favicon.ico">
<link rel="apple-touch-icon" href="apple-touch-icon.png">

<!-- Open Graph / redes sociales -->
<meta property="og:type" content="website">
<meta property="og:title" content="OBRA — Estudio de Arquitectura">
<meta property="og:description" content="Diseñamos espacios simples, auténticos y cercanos a la naturaleza. Arquitectura, interiorismo y planificación a medida.">
<meta property="og:image" content="og-image.png">
<meta property="og:locale" content="es_LA">
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="OBRA — Estudio de Arquitectura">
<meta name="twitter:description" content="Diseñamos espacios simples, auténticos y cercanos a la naturaleza.">
<meta name="twitter:image" content="og-image.png">
<meta name="theme-color" content="#ECE9E1">
<meta name="robots" content="index, follow">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,300;0,9..144,400;0,9..144,500;0,9..144,600;1,9..144,400&family=Inter:wght@400;500;600&family=Space+Mono:wght@400;700&display=swap" rel="stylesheet">
<style>
/* ============================================================
   OBRA — Estudio de Arquitectura
   Tokens: papel piedra + tinta + azul de plano + bronce
   ============================================================ */

:root{
  --paper:      #ECE9E1;
  --paper-2:    #E2DED2;
  --ink:        #1B1D1E;
  --ink-soft:   #55534C;
  --line:       #C7C0AF;
  --line-soft:  #D8D3C4;
  --blue:       #2C4A5E;
  --blue-deep:  #14242E;
  --brass:      #9C6B37;
  --white:      #FAF8F4;

  --serif: 'Fraunces', 'Iowan Old Style', serif;
  --sans:  'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  --mono:  'Space Mono', 'SFMono-Regular', monospace;

  --max: 1180px;
  --pad: clamp(20px, 5vw, 64px);
}

*, *::before, *::after{ box-sizing: border-box; }
html{ scroll-behavior: smooth; }
@media (prefers-reduced-motion: reduce){
  html{ scroll-behavior: auto; }
  *, *::before, *::after{ animation-duration: 0.001ms !important; animation-iteration-count: 1 !important; transition-duration: 0.001ms !important; }
}

body{
  margin:0;
  background: var(--paper);
  color: var(--ink);
  font-family: var(--sans);
  font-size: 16px;
  line-height: 1.6;
  -webkit-font-smoothing: antialiased;
}

img, svg{ display:block; max-width:100%; }
a{ color: inherit; text-decoration:none; }
ul{ list-style:none; margin:0; padding:0; }
h1,h2,h3,h4{ font-family: var(--serif); font-weight:500; margin:0; color: var(--ink); }
p{ margin:0; }

a:focus-visible, button:focus-visible, input:focus-visible, textarea:focus-visible{
  outline: 2px solid var(--blue);
  outline-offset: 3px;
}

.skip-link{
  position:absolute; left:-9999px; top:auto;
  background: var(--ink); color:var(--white); padding:10px 16px; z-index:200;
}
.skip-link:focus{ left:16px; top:16px; }

.eyebrow{
  font-family: var(--mono);
  font-size: 12.5px;
  letter-spacing: .08em;
  text-transform: uppercase;
  color: var(--brass);
  margin: 0 0 14px;
}

.btn{
  display:inline-flex; align-items:center; gap:8px;
  font-family: var(--mono);
  font-size: 13px;
  letter-spacing:.03em;
  text-transform: uppercase;
  padding: 13px 26px;
  border-radius: 2px;
  transition: background .2s ease, color .2s ease, border-color .2s ease;
  cursor:pointer;
  border: 1px solid transparent;
}
.btn-solid{ background: var(--ink); color: var(--white); }
.btn-solid:hover{ background: var(--blue); }
.btn-line{ border-color: var(--ink); color: var(--ink); background:transparent; }
.btn-line:hover{ background: var(--ink); color: var(--white); }
.btn-text{ padding: 13px 4px; color: var(--ink); }
.btn-text:hover{ color: var(--brass); }

/* ================= HEADER ================= */
.site-header{
  position: sticky; top:0; z-index:100;
  background: rgba(236,233,225,.92);
  backdrop-filter: blur(6px);
  border-bottom: 1px solid var(--line);
}
.header-inner{
  max-width: var(--max); margin:0 auto; padding: 16px var(--pad);
  display:flex; align-items:center; gap: 32px;
}
.brand{ display:flex; align-items:center; gap:10px; margin-right:auto; }
.brand-mark{ color: var(--ink); display:flex; }
.brand-name{
  font-family: var(--serif); font-size: 19px; letter-spacing:.02em; font-weight:600;
  display:flex; flex-direction:column; line-height:1.05;
}
.brand-suffix{ font-family: var(--mono); font-size:9.5px; letter-spacing:.12em; text-transform:uppercase; color: var(--ink-soft); font-weight:400; }

.main-nav ul{ display:flex; gap: 30px; }
.nav-link{
  font-family: var(--mono); font-size: 12.5px; letter-spacing:.04em; text-transform:uppercase;
  color: var(--ink-soft);
  position:relative; padding-bottom:4px;
}
.nav-link::after{
  content:''; position:absolute; left:0; bottom:0; width:0; height:1px; background: var(--brass);
  transition: width .25s ease;
}
.nav-link:hover, .nav-link.active{ color: var(--ink); }
.nav-link:hover::after, .nav-link.active::after{ width:100%; }

.header-cta{ flex-shrink:0; }

.nav-toggle{
  display:none; flex-direction:column; justify-content:center; gap:5px;
  width:36px; height:36px; background:none; border:none; cursor:pointer; padding:0;
}
.nav-toggle span{ display:block; width:100%; height:2px; background: var(--ink); transition: transform .25s ease, opacity .25s ease; }
.nav-toggle[aria-expanded="true"] span:nth-child(1){ transform: translateY(7px) rotate(45deg); }
.nav-toggle[aria-expanded="true"] span:nth-child(2){ opacity:0; }
.nav-toggle[aria-expanded="true"] span:nth-child(3){ transform: translateY(-7px) rotate(-45deg); }

/* ================= HERO ================= */
.hero{
  position:relative; overflow:hidden;
  display:grid; grid-template-columns: 1.05fr .95fr; align-items:center; gap: 40px;
  max-width: var(--max); margin:0 auto; padding: clamp(50px,9vw,110px) var(--pad) clamp(60px,8vw,90px);
}
.hero-grid{
  position:absolute; inset:0;
  background-image:
    linear-gradient(var(--line-soft) 1px, transparent 1px),
    linear-gradient(90deg, var(--line-soft) 1px, transparent 1px);
  background-size: 42px 42px;
  mask-image: radial-gradient(ellipse 80% 60% at 30% 20%, black, transparent 75%);
  opacity:.55;
  z-index:0;
}
.hero-inner{ position:relative; z-index:1; }
.hero-title{
  font-size: clamp(2.6rem, 5.2vw, 4.4rem);
  line-height: 1.04;
  letter-spacing:-.01em;
  margin-bottom: 26px;
}
.hero-title em{ font-style:italic; color: var(--blue); }
.hero-copy{ max-width: 46ch; color: var(--ink-soft); font-size: 1.05rem; margin-bottom: 34px; }
.hero-actions{ display:flex; align-items:center; gap: 28px; flex-wrap:wrap; }

.hero-drawing{ position:relative; z-index:1; }
.elevation-svg{ width:100%; height:auto; color: var(--blue-deep); }
.draw-line{
  fill:none; stroke: currentColor; stroke-width:2;
  stroke-dasharray: var(--d); stroke-dashoffset: var(--d);
  animation: draw 1.1s ease forwards;
  animation-delay: var(--delay);
}
.draw-line.thin{ stroke-width:1.2; color: var(--brass); }
.draw-line.dashed{ stroke-dasharray: 4 5; stroke-dashoffset:0; animation:none; opacity:.7; }
@keyframes draw{ to{ stroke-dashoffset:0; } }
.drawing-tag{
  display:block; margin-top:14px; text-align:right;
  font-family: var(--mono); font-size:11px; letter-spacing:.05em; text-transform:uppercase;
  color: var(--ink-soft);
}

/* ================= SECTIONS ================= */
.section{ padding: clamp(64px,9vw,110px) 0; }
.section-alt{ background: var(--paper-2); }
.section-dark{
  background: var(--blue-deep); color: var(--white);
  padding: clamp(50px,7vw,80px) 0;
}
.section-inner{ max-width: var(--max); margin:0 auto; padding: 0 var(--pad); }
.grid-2{ display:grid; grid-template-columns: .85fr 1.15fr; gap: clamp(40px,6vw,90px); align-items:start; }

.section-head{ max-width: 640px; }
.section-head.center{ max-width: 640px; margin: 0 auto 56px; text-align:center; }
.section-title{ font-size: clamp(1.9rem, 3.4vw, 2.6rem); line-height:1.12; margin-bottom: 18px; }
.section-copy{ color: var(--ink-soft); max-width: 46ch; }
.section-head.center .section-copy{ margin:0 auto; }

/* feature list (Estudio) */
.feature-list{ display:flex; flex-direction:column; gap: 30px; }
.feature-item{ display:flex; gap: 22px; padding-top: 26px; border-top: 1px solid var(--line); }
.feature-item:first-child{ border-top:none; padding-top:0; }
.feature-index{ font-family: var(--mono); font-size: 13px; color: var(--brass); padding-top:4px; }
.feature-item h3{ font-size: 1.15rem; margin-bottom:8px; }
.feature-item p{ color: var(--ink-soft); max-width: 44ch; }

/* services grid */
.service-grid{ display:grid; grid-template-columns: repeat(3, 1fr); gap: 1px; background: var(--line); border:1px solid var(--line); }
.service-card{ background: var(--paper-2); padding: 34px 28px; }
.service-icon{ width:34px; height:34px; color: var(--blue); margin-bottom: 20px; }
.service-card h3{ font-size: 1.05rem; margin-bottom:8px; }
.service-card p{ color: var(--ink-soft); font-size:.95rem; }

/* portfolio */
.portfolio-grid{ display:grid; grid-template-columns: repeat(3, 1fr); gap: 28px; }
.portfolio-card{ cursor:default; }
.portfolio-thumb{
  background: var(--white); border:1px solid var(--line); overflow:hidden; margin-bottom: 16px;
  transition: border-color .2s ease;
}
.portfolio-card:hover .portfolio-thumb{ border-color: var(--brass); }
.plan-bg{ fill: var(--white); }
.plan-line{ fill:none; stroke: var(--blue-deep); stroke-width:1.6; }
.plan-line.thin{ stroke: var(--brass); stroke-width:1; }
.portfolio-tag{ font-family: var(--mono); font-size:11px; letter-spacing:.05em; text-transform:uppercase; color: var(--brass); margin-bottom:6px; }
.portfolio-card h3{ font-size:1.05rem; }

/* stats */
.stats-grid{ display:grid; grid-template-columns: repeat(4,1fr); gap: 30px; text-align:center; }
.stat-number{ display:block; font-family: var(--serif); font-size: clamp(2.2rem,4vw,3rem); color: var(--white); }
.stat-label{ font-family: var(--mono); font-size:12px; letter-spacing:.05em; text-transform:uppercase; color: rgba(250,248,244,.6); }

/* testimonials */
.testimonial-grid{ display:grid; grid-template-columns: repeat(3,1fr); gap: 30px; }
.testimonial{ background: var(--paper-2); border-left: 2px solid var(--brass); padding: 28px 26px; margin:0; }
.testimonial p{ font-family: var(--serif); font-style:italic; font-size:1.05rem; line-height:1.5; margin-bottom: 20px; color: var(--ink); }
.testimonial footer{ display:flex; flex-direction:column; }
.testimonial cite{ font-style:normal; font-family: var(--mono); font-size:12.5px; letter-spacing:.03em; }
.testimonial footer span{ color: var(--ink-soft); font-size:.85rem; }

/* blog */
.blog-grid{ display:grid; grid-template-columns: repeat(3,1fr); gap: 30px; }
.blog-card{ padding-top: 20px; border-top:1px solid var(--line); }
.blog-meta{ font-family: var(--mono); font-size:11px; letter-spacing:.04em; text-transform:uppercase; color: var(--brass); margin-bottom:12px; }
.blog-card h3{ font-size:1.1rem; margin-bottom:10px; line-height:1.3; }
.blog-card p{ color: var(--ink-soft); font-size:.95rem; }

/* contact */
.contact-list{ margin-top: 28px; display:flex; flex-direction:column; gap:14px; }
.contact-list li{ font-size:.98rem; }
.contact-list span{ display:block; font-family: var(--mono); font-size:11px; letter-spacing:.05em; text-transform:uppercase; color: var(--brass); margin-bottom:2px; }
.contact-list a:hover{ color: var(--blue); }

.contact-form{ background: var(--white); border:1px solid var(--line); padding: clamp(24px,4vw,40px); }
.form-row{ display:flex; flex-direction:column; gap:6px; margin-bottom: 20px; }
.form-row label{ font-family: var(--mono); font-size:11.5px; letter-spacing:.04em; text-transform:uppercase; color: var(--ink-soft); }
.form-row input, .form-row textarea{
  font-family: var(--sans); font-size:1rem; padding: 12px 14px;
  border: 1px solid var(--line); background: var(--paper); color: var(--ink);
  border-radius:2px; resize:vertical;
}
.form-row input:focus, .form-row textarea:focus{ border-color: var(--blue); }
.form-note{ margin-top:14px; font-size:.9rem; color: var(--blue); min-height:1.2em; }

/* ================= FOOTER ================= */
.site-footer{ background: var(--blue-deep); color: rgba(250,248,244,.85); }
.footer-inner{
  max-width: var(--max); margin:0 auto; padding: 64px var(--pad) 40px;
  display:grid; grid-template-columns: 1.4fr 1fr 1fr 1fr; gap: 40px;
}
.site-footer .brand{ color: var(--white); margin-bottom: 16px; }
.site-footer .brand-suffix{ color: rgba(250,248,244,.55); }
.footer-col p{ color: rgba(250,248,244,.6); font-size:.92rem; max-width:32ch; }
.footer-col h4{ font-family: var(--mono); font-size:12px; letter-spacing:.06em; text-transform:uppercase; color: var(--brass); margin-bottom:16px; font-weight:400; }
.footer-col ul{ display:flex; flex-direction:column; gap:10px; }
.footer-col a{ color: rgba(250,248,244,.75); font-size:.92rem; }
.footer-col a:hover{ color: var(--white); }
.social-row{ display:flex; gap:14px; }
.social-row a{
  width:34px; height:34px; border:1px solid rgba(250,248,244,.3); border-radius:50%;
  display:flex; align-items:center; justify-content:center; font-family: var(--mono); font-size:11px;
}
.social-row a:hover{ background: var(--brass); border-color: var(--brass); }
.footer-bottom{ border-top:1px solid rgba(250,248,244,.15); padding: 18px var(--pad); }
.footer-bottom p{ font-size:.85rem; color: rgba(250,248,244,.55); max-width: var(--max); margin:0 auto; }

/* ================= RESPONSIVE ================= */
@media (max-width: 980px){
  .hero{ grid-template-columns:1fr; }
  .hero-drawing{ order:-1; max-width: 420px; }
  .grid-2{ grid-template-columns:1fr; }
  .service-grid, .portfolio-grid, .testimonial-grid, .blog-grid{ grid-template-columns: repeat(2,1fr); }
  .stats-grid{ grid-template-columns: repeat(2,1fr); row-gap: 34px; }
  .footer-inner{ grid-template-columns: 1fr 1fr; }
}

@media (max-width: 760px){
  .main-nav{
    position: fixed; inset: 64px 0 0 0; background: var(--paper);
    transform: translateY(-8px); opacity:0; pointer-events:none;
    transition: opacity .2s ease, transform .2s ease;
    border-top: 1px solid var(--line);
    overflow-y:auto;
  }
  .main-nav.open{ opacity:1; transform:translateY(0); pointer-events:auto; }
  .main-nav ul{ flex-direction:column; gap:0; padding: 10px var(--pad); }
  .main-nav li{ border-bottom:1px solid var(--line); }
  .main-nav .nav-link{ display:block; padding: 16px 0; font-size:14px; }
  .header-cta{ display:none; }
  .nav-toggle{ display:flex; }
  .service-grid, .portfolio-grid, .testimonial-grid, .blog-grid{ grid-template-columns: 1fr; }
  .stats-grid{ grid-template-columns: 1fr 1fr; }
  .footer-inner{ grid-template-columns: 1fr; }
}

</style>
</head>
<body>

<a class="skip-link" href="#contenido">Saltar al contenido</a>

<!-- ===== HEADER ===== -->
<header class="site-header" id="top">
  <div class="header-inner">
    <a href="#top" class="brand">
      <span class="brand-mark" aria-hidden="true">
        <svg viewBox="0 0 40 40" width="34" height="34">
          <path d="M4 32 L20 8 L36 32" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linejoin="round" stroke-linecap="round"/>
          <line x1="10" y1="32" x2="10" y2="22" stroke="currentColor" stroke-width="2.5"/>
          <line x1="30" y1="32" x2="30" y2="22" stroke="currentColor" stroke-width="2.5"/>
        </svg>
      </span>
      <span class="brand-name">OBRA<span class="brand-suffix">Arquitectura</span></span>
    </a>

    <nav class="main-nav" id="main-nav" aria-label="Navegación principal">
      <ul>
        <li><a href="#estudio" class="nav-link">Estudio</a></li>
        <li><a href="#enfoque" class="nav-link">Enfoque</a></li>
        <li><a href="#proyectos" class="nav-link">Proyectos</a></li>
        <li><a href="#cifras" class="nav-link">Cifras</a></li>
        <li><a href="#testimonios" class="nav-link">Testimonios</a></li>
        <li><a href="#bitacora" class="nav-link">Bitácora</a></li>
      </ul>
    </nav>

    <a href="#contacto" class="btn btn-line header-cta">Contáctanos</a>

    <button class="nav-toggle" id="navToggle" aria-expanded="false" aria-controls="main-nav" aria-label="Abrir menú">
      <span></span><span></span><span></span>
    </button>
  </div>
</header>

<main id="contenido">

  <!-- ===== HERO ===== -->
  <section class="hero" id="hero">
    <div class="hero-grid" aria-hidden="true"></div>
    <div class="hero-inner">
      <p class="eyebrow">A-01 &nbsp;/&nbsp; Presentación</p>
      <h1 class="hero-title">
        Simple.<br>
        Auténtica.<br>
        <em>Cercana a la naturaleza.</em>
      </h1>
      <p class="hero-copy">
        Diseñamos espacios que envejecen bien: volúmenes claros, materiales honestos
        y una relación cuidada con la luz y el terreno. Cada proyecto empieza en el
        mismo lugar — escuchando cómo se quiere vivir ese espacio.
      </p>
      <div class="hero-actions">
        <a href="#proyectos" class="btn btn-solid">Ver proyectos</a>
        <a href="#estudio" class="btn btn-text">Conocer el estudio →</a>
      </div>
    </div>

    <div class="hero-drawing" aria-hidden="true">
      <svg viewBox="0 0 520 420" class="elevation-svg">
        <!-- ground line -->
        <line x1="20" y1="380" x2="500" y2="380" class="draw-line" style="--d:900; --delay:0s"/>
        <!-- main volume -->
        <path d="M60 380 L60 160 L280 160 L280 380" class="draw-line" style="--d:760; --delay:.1s"/>
        <!-- roof pitch -->
        <path d="M40 160 L170 70 L300 160" class="draw-line" style="--d:420; --delay:.4s"/>
        <!-- secondary volume -->
        <path d="M280 380 L280 240 L420 240 L420 380" class="draw-line" style="--d:520; --delay:.55s"/>
        <!-- windows -->
        <rect x="95" y="220" width="55" height="70" class="draw-line thin" style="--d:250; --delay:.9s"/>
        <rect x="190" y="220" width="55" height="70" class="draw-line thin" style="--d:250; --delay:1s"/>
        <rect x="320" y="280" width="60" height="60" class="draw-line thin" style="--d:240; --delay:1.1s"/>
        <!-- door -->
        <rect x="130" y="320" width="40" height="60" class="draw-line thin" style="--d:200; --delay:1.2s"/>
        <!-- dimension marks -->
        <line x1="20" y1="380" x2="20" y2="400" class="draw-line thin" style="--d:20; --delay:1.3s"/>
        <line x1="500" y1="380" x2="500" y2="400" class="draw-line thin" style="--d:20; --delay:1.3s"/>
        <line x1="20" y1="398" x2="500" y2="398" class="draw-line thin dashed" style="--d:480; --delay:1.35s"/>
      </svg>
      <span class="drawing-tag">FIG. 01 — Elevación frontal, s/e</span>
    </div>
  </section>

  <!-- ===== ESTUDIO / ABOUT ===== -->
  <section class="section" id="estudio">
    <div class="section-inner grid-2">
      <div class="section-head">
        <p class="eyebrow">A-02 &nbsp;/&nbsp; El estudio</p>
        <h2 class="section-title">Un boceto de<br>cada detalle</h2>
        <p class="section-copy">
          Nuestra filosofía es sencilla: cada encargo merece una solución propia,
          pensada desde cero. Desarrollamos los proyectos con rapidez sin perder
          el detalle — desde el primer boceto hasta el plano de obra.
        </p>
      </div>

      <div class="feature-list">
        <article class="feature-item">
          <span class="feature-index">01</span>
          <div>
            <h3>Visualización 3D</h3>
            <p>Modelamos cada ambiente antes de construirlo, para decidir con certeza y no con suposiciones.</p>
          </div>
        </article>
        <article class="feature-item">
          <span class="feature-index">02</span>
          <div>
            <h3>Proyecto individual</h3>
            <p>Ningún diseño se repite. Partimos del terreno, el clima y quienes van a habitarlo.</p>
          </div>
        </article>
        <article class="feature-item">
          <span class="feature-index">03</span>
          <div>
            <h3>Planificación 2D</h3>
            <p>Plantas y cortes técnicos listos para permisos, presupuesto y obra — sin sorpresas a mitad de camino.</p>
          </div>
        </article>
      </div>
    </div>
  </section>

  <!-- ===== ENFOQUE / SERVICIOS ===== -->
  <section class="section section-alt" id="enfoque">
    <div class="section-inner">
      <div class="section-head center">
        <p class="eyebrow">A-03 &nbsp;/&nbsp; Enfoque</p>
        <h2 class="section-title">Qué podemos<br>ofrecerte</h2>
      </div>

      <div class="service-grid">
        <article class="service-card">
          <svg class="service-icon" viewBox="0 0 48 48" aria-hidden="true"><path d="M6 40 L24 8 L42 40 Z M16 40 L16 26 L32 26 L32 40" fill="none" stroke="currentColor" stroke-width="1.6"/></svg>
          <h3>Diseño &amp; Planificación</h3>
          <p>Te acompañamos desde el primer croquis hasta el proyecto ejecutivo.</p>
        </article>
        <article class="service-card">
          <svg class="service-icon" viewBox="0 0 48 48" aria-hidden="true"><rect x="8" y="8" width="32" height="32" fill="none" stroke="currentColor" stroke-width="1.6"/><path d="M8 24 L40 24 M24 8 L24 40" stroke="currentColor" stroke-width="1.6"/></svg>
          <h3>Soluciones a medida</h3>
          <p>Respuestas concretas a terrenos difíciles, presupuestos ajustados o programas complejos.</p>
        </article>
        <article class="service-card">
          <svg class="service-icon" viewBox="0 0 48 48" aria-hidden="true"><path d="M10 34 L10 18 L24 10 L38 18 L38 34 Z" fill="none" stroke="currentColor" stroke-width="1.6"/><line x1="24" y1="22" x2="24" y2="34" stroke="currentColor" stroke-width="1.6"/></svg>
          <h3>Mobiliario &amp; Decoración</h3>
          <p>Piezas y ambientaciones diseñadas junto con el espacio, no añadidas después.</p>
        </article>
        <article class="service-card">
          <svg class="service-icon" viewBox="0 0 48 48" aria-hidden="true"><circle cx="24" cy="24" r="16" fill="none" stroke="currentColor" stroke-width="1.6"/><path d="M24 8 L24 24 L34 30" stroke="currentColor" stroke-width="1.6" fill="none"/></svg>
          <h3>Diseño Exterior</h3>
          <p>Fachadas, paisajismo y espacios de transición entre lo construido y el terreno.</p>
        </article>
        <article class="service-card">
          <svg class="service-icon" viewBox="0 0 48 48" aria-hidden="true"><path d="M8 30 Q24 8 40 30" fill="none" stroke="currentColor" stroke-width="1.6"/><circle cx="24" cy="30" r="3" fill="currentColor"/></svg>
          <h3>Creación de Concepto</h3>
          <p>Partimos de una idea rectora clara que ordena cada decisión posterior.</p>
        </article>
        <article class="service-card">
          <svg class="service-icon" viewBox="0 0 48 48" aria-hidden="true"><path d="M14 34 L34 14 M14 14 L34 34" stroke="currentColor" stroke-width="1.6"/><circle cx="24" cy="24" r="18" fill="none" stroke="currentColor" stroke-width="1.6"/></svg>
          <h3>Control de Autor</h3>
          <p>Supervisamos la obra para que lo construido sea fiel al proyecto original.</p>
        </article>
      </div>
    </div>
  </section>

  <!-- ===== PROYECTOS / PORTFOLIO ===== -->
  <section class="section" id="proyectos">
    <div class="section-inner">
      <div class="section-head center">
        <p class="eyebrow">A-04 &nbsp;/&nbsp; Proyectos</p>
        <h2 class="section-title">Trabajo reciente</h2>
      </div>

      <div class="portfolio-grid">

        <article class="portfolio-card">
          <div class="portfolio-thumb">
            <svg viewBox="0 0 300 220"><rect width="300" height="220" class="plan-bg"/><path d="M40 180 L40 60 L180 60 L180 110 L260 110 L260 180 Z" class="plan-line"/><line x1="40" y1="130" x2="180" y2="130" class="plan-line thin"/></svg>
          </div>
          <p class="portfolio-tag">Interiorismo</p>
          <h3>Departamento Familiar</h3>
        </article>

        <article class="portfolio-card">
          <div class="portfolio-thumb">
            <svg viewBox="0 0 300 220"><rect width="300" height="220" class="plan-bg"/><path d="M60 40 L60 190 L230 190 L230 100 L150 100 L150 40 Z" class="plan-line"/><rect x="90" y="150" width="30" height="40" class="plan-line thin"/></svg>
          </div>
          <p class="portfolio-tag">Decoración · Interiorismo</p>
          <h3>Casa de Huéspedes</h3>
        </article>

        <article class="portfolio-card">
          <div class="portfolio-thumb">
            <svg viewBox="0 0 300 220"><rect width="300" height="220" class="plan-bg"/><path d="M40 190 L100 60 L160 190 Z" class="plan-line"/><path d="M160 190 L160 100 L250 100 L250 190" class="plan-line"/></svg>
          </div>
          <p class="portfolio-tag">Arquitectura</p>
          <h3>Residencia de Autor</h3>
        </article>

        <article class="portfolio-card">
          <div class="portfolio-thumb">
            <svg viewBox="0 0 300 220"><rect width="300" height="220" class="plan-bg"/><rect x="60" y="60" width="180" height="120" class="plan-line"/><line x1="150" y1="60" x2="150" y2="180" class="plan-line thin"/><line x1="60" y1="120" x2="240" y2="120" class="plan-line thin"/></svg>
          </div>
          <p class="portfolio-tag">Mobiliario</p>
          <h3>Casa en España</h3>
        </article>

        <article class="portfolio-card">
          <div class="portfolio-thumb">
            <svg viewBox="0 0 300 220"><rect width="300" height="220" class="plan-bg"/><path d="M50 180 L50 70 L250 70 L250 180 Z" class="plan-line"/><path d="M50 70 L150 30 L250 70" class="plan-line"/></svg>
          </div>
          <p class="portfolio-tag">Mobiliario</p>
          <h3>Villa Moderna en Bélgica</h3>
        </article>

        <article class="portfolio-card">
          <div class="portfolio-thumb">
            <svg viewBox="0 0 300 220"><rect width="300" height="220" class="plan-bg"/><rect x="70" y="50" width="160" height="140" class="plan-line"/><circle cx="150" cy="120" r="30" class="plan-line thin"/></svg>
          </div>
          <p class="portfolio-tag">Interiorismo</p>
          <h3>Departamento Minimalista</h3>
        </article>

      </div>
    </div>
  </section>

  <!-- ===== CIFRAS / STATS ===== -->
  <section class="section section-dark" id="cifras">
    <div class="section-inner">
      <div class="stats-grid">
        <div class="stat">
          <span class="stat-number" data-count="120">0</span>
          <span class="stat-label">Clientes activos</span>
        </div>
        <div class="stat">
          <span class="stat-number" data-count="14">0</span>
          <span class="stat-label">Años de experiencia</span>
        </div>
        <div class="stat">
          <span class="stat-number" data-count="9">0</span>
          <span class="stat-label">Premios recibidos</span>
        </div>
        <div class="stat">
          <span class="stat-number" data-count="3">0</span>
          <span class="stat-label">Oficinas en el mundo</span>
        </div>
      </div>
    </div>
  </section>

  <!-- ===== TESTIMONIOS ===== -->
  <section class="section" id="testimonios">
    <div class="section-inner">
      <div class="section-head center">
        <p class="eyebrow">A-05 &nbsp;/&nbsp; Testimonios</p>
        <h2 class="section-title">Lo que dicen<br>nuestros clientes</h2>
      </div>

      <div class="testimonial-grid">
        <blockquote class="testimonial">
          <p>“Nunca vas a fingir la sensación de estar en un lugar así. Un minimalismo vivo, apoyado en materiales naturales y texturas sin procesar: auténtico, con memoria propia.”</p>
          <footer><cite>Pablo Guisado</cite><span>Cliente del estudio</span></footer>
        </blockquote>
        <blockquote class="testimonial">
          <p>“Nos acompañaron en cada decisión, incluso las que no sabíamos que teníamos que tomar. El resultado final superó lo que habíamos imaginado al empezar.”</p>
          <footer><cite>Ana Paulina</cite><span>Cliente del estudio</span></footer>
        </blockquote>
        <blockquote class="testimonial">
          <p>“Un equipo ordenado, puntual con los plazos y honesto con los costos. Justo lo que buscábamos para un proyecto de esta escala.”</p>
          <footer><cite>Cristina Lee</cite><span>Cliente del estudio</span></footer>
        </blockquote>
      </div>
    </div>
  </section>

  <!-- ===== BITÁCORA / BLOG ===== -->
  <section class="section section-alt" id="bitacora">
    <div class="section-inner">
      <div class="section-head center">
        <p class="eyebrow">A-06 &nbsp;/&nbsp; Bitácora</p>
        <h2 class="section-title">Notas del estudio</h2>
      </div>

      <div class="blog-grid">
        <article class="blog-card">
          <p class="blog-meta">Interiorismo · 20 marzo 2026</p>
          <h3>Diez decisiones clave para una cocina que funcione</h3>
          <p>El orden de una cocina se define antes del mobiliario: primero el recorrido, después los muebles.</p>
        </article>
        <article class="blog-card">
          <p class="blog-meta">Arquitectura · 20 marzo 2026</p>
          <h3>La proporción áurea aplicada a un buen boceto 2D</h3>
          <p>Una proporción bien elegida se nota incluso antes de entender por qué funciona.</p>
        </article>
        <article class="blog-card">
          <p class="blog-meta">Interiorismo · 19 marzo 2026</p>
          <h3>Colores tierra y materiales naturales</h3>
          <p>Una paleta reducida, bien elegida, envejece mejor que cualquier tendencia de temporada.</p>
        </article>
      </div>
    </div>
  </section>

  <!-- ===== CONTACTO ===== -->
  <section class="section" id="contacto">
    <div class="section-inner grid-2">
      <div class="section-head">
        <p class="eyebrow">A-07 &nbsp;/&nbsp; Contacto</p>
        <h2 class="section-title">Conversemos<br>sobre tu proyecto</h2>
        <p class="section-copy">
          Contanos qué estás por construir o remodelar. Respondemos en menos de 48 horas hábiles.
        </p>
        <ul class="contact-list">
          <li><span>Dirección</span> Av. Mariscal López 1234, Asunción, Paraguay</li>
          <li><span>Correo</span> <a href="mailto:hola@obraarquitectura.com">hola@obraarquitectura.com</a></li>
          <li><span>Teléfono</span> <a href="tel:+595210000000">+595 21 000 0000</a></li>
        </ul>
      </div>

      <form class="contact-form" id="contactForm">
        <div class="form-row">
          <label for="nombre">Nombre</label>
          <input type="text" id="nombre" name="nombre" required>
        </div>
        <div class="form-row">
          <label for="email">Correo</label>
          <input type="email" id="email" name="email" required>
        </div>
        <div class="form-row">
          <label for="mensaje">Contanos sobre tu proyecto</label>
          <textarea id="mensaje" name="mensaje" rows="4" required></textarea>
        </div>
        <button type="submit" class="btn btn-solid">Enviar mensaje</button>
        <p class="form-note" id="formNote" role="status"></p>
      </form>
    </div>
  </section>

</main>

<!-- ===== FOOTER ===== -->
<footer class="site-footer">
  <div class="footer-inner">
    <div class="footer-col">
      <a href="#top" class="brand">
        <span class="brand-mark" aria-hidden="true">
          <svg viewBox="0 0 40 40" width="30" height="30">
            <path d="M4 32 L20 8 L36 32" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linejoin="round" stroke-linecap="round"/>
          </svg>
        </span>
        <span class="brand-name">OBRA</span>
      </a>
      <p>Un equipo compacto de personas con oficios distintos, trabajando sobre el mismo plano.</p>
    </div>

    <div class="footer-col">
      <h4>Contacto</h4>
      <ul>
        <li>Av. Mariscal López 1234, Asunción, Paraguay</li>
        <li><a href="mailto:hola@obraarquitectura.com">hola@obraarquitectura.com</a></li>
        <li><a href="tel:+595210000000">+595 21 000 0000</a></li>
      </ul>
    </div>

    <div class="footer-col">
      <h4>Proyectos recientes</h4>
      <ul>
        <li><a href="#proyectos">Departamento Familiar</a></li>
        <li><a href="#proyectos">Villa Moderna en Bélgica</a></li>
        <li><a href="#proyectos">Casa en España</a></li>
      </ul>
    </div>

    <div class="footer-col">
      <h4>Seguinos</h4>
      <div class="social-row">
        <a href="#" aria-label="Facebook">FB</a>
        <a href="#" aria-label="Instagram">IG</a>
        <a href="#" aria-label="LinkedIn">IN</a>
      </div>
    </div>
  </div>
  <div class="footer-bottom">
    <p>© 2026 OBRA Arquitectura. Todos los derechos reservados.</p>
  </div>
</footer>

<script>
// ===== Menú móvil =====
const navToggle = document.getElementById('navToggle');
const mainNav = document.getElementById('main-nav');

navToggle.addEventListener('click', () => {
  const isOpen = mainNav.classList.toggle('open');
  navToggle.setAttribute('aria-expanded', String(isOpen));
  navToggle.setAttribute('aria-label', isOpen ? 'Cerrar menú' : 'Abrir menú');
});

document.querySelectorAll('.nav-link').forEach(link => {
  link.addEventListener('click', () => {
    mainNav.classList.remove('open');
    navToggle.setAttribute('aria-expanded', 'false');
  });
});

// ===== Resaltar enlace activo según la sección visible =====
const sections = document.querySelectorAll('main section[id]');
const navLinks = document.querySelectorAll('.nav-link');

const setActive = (id) => {
  navLinks.forEach(link => {
    link.classList.toggle('active', link.getAttribute('href') === `#${id}`);
  });
};

const sectionObserver = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) setActive(entry.target.id);
  });
}, { rootMargin: '-45% 0px -50% 0px', threshold: 0 });

sections.forEach(section => sectionObserver.observe(section));

// ===== Contadores animados (sección Cifras) =====
const statNumbers = document.querySelectorAll('.stat-number');

const animateCount = (el) => {
  const target = parseInt(el.dataset.count, 10);
  const duration = 1400;
  const start = performance.now();

  const step = (now) => {
    const progress = Math.min((now - start) / duration, 1);
    const eased = 1 - Math.pow(1 - progress, 3);
    el.textContent = Math.round(eased * target);
    if (progress < 1) requestAnimationFrame(step);
  };
  requestAnimationFrame(step);
};

const statObserver = new IntersectionObserver((entries, observer) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      animateCount(entry.target);
      observer.unobserve(entry.target);
    }
  });
}, { threshold: 0.6 });

statNumbers.forEach(el => statObserver.observe(el));

// ===== Formulario de contacto (demo estática, sin backend) =====
const contactForm = document.getElementById('contactForm');
const formNote = document.getElementById('formNote');

if (contactForm) {
  contactForm.addEventListener('submit', (e) => {
    e.preventDefault();
    formNote.textContent = 'Gracias — este formulario es una demo estática. Conectalo a tu backend o a un servicio como Formspree para recibir mensajes reales.';
  });
}

</script>
</body>
</html>
