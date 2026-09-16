<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Nombre Empresa | Soluciones profesionales</title>
<meta name="description" content="Plantilla de sitio web bilingue espanol / ingles.">
<style>
  :root{
    --brand:#0a4d68;
    --brand-2:#0f7ea1;
    --accent:#f6a21d;
    --ink:#16222b;
    --muted:#5a6a75;
    --line:#e2e8ec;
    --bg:#ffffff;
    --bg-soft:#f5f8fa;
    --radius:10px;
    --max:1120px;
    --font:"Segoe UI",system-ui,-apple-system,Roboto,Helvetica,Arial,sans-serif;
  }
  *{box-sizing:border-box;margin:0;padding:0}
  html{scroll-behavior:smooth}
  body{font-family:var(--font);color:var(--ink);background:var(--bg);line-height:1.6;font-size:16px}
  img{max-width:100%;display:block}
  a{color:inherit;text-decoration:none}
  .wrap{max-width:var(--max);margin:0 auto;padding:0 24px}

  /* ---------- HEADER ---------- */
  header{position:sticky;top:0;z-index:50;background:rgba(255,255,255,.96);
    backdrop-filter:blur(6px);border-bottom:1px solid var(--line)}
  .bar{display:flex;align-items:center;justify-content:space-between;gap:16px;
    max-width:var(--max);margin:0 auto;padding:14px 24px;position:relative}
  .logo{display:flex;align-items:center;gap:10px;font-weight:700;font-size:1.05rem;letter-spacing:.2px}
  .logo svg{width:40px;height:40px;flex:none}
  .logo small{display:block;font-weight:400;font-size:.7rem;color:var(--muted);letter-spacing:1.6px;text-transform:uppercase}

  nav ul{display:flex;list-style:none;gap:28px;align-items:center}
  nav a{font-size:.94rem;font-weight:500;color:var(--muted);padding:6px 0;border-bottom:2px solid transparent;transition:.2s}
  nav a:hover,nav a.active{color:var(--brand);border-color:var(--accent)}

  .lang{display:flex;border:1px solid var(--line);border-radius:999px;overflow:hidden;flex:none}
  .lang button{border:0;background:transparent;padding:6px 13px;font:inherit;font-size:.8rem;
    font-weight:600;color:var(--muted);cursor:pointer;transition:.2s}
  .lang button.on{background:var(--brand);color:#fff}

  .burger{display:none;border:1px solid var(--line);background:#fff;border-radius:8px;
    padding:8px 11px;font-size:1.1rem;cursor:pointer;line-height:1}

  /* ---------- HERO ---------- */
  .hero{background:linear-gradient(135deg,var(--brand) 0%,var(--brand-2) 100%);color:#fff;
    padding:96px 0 88px;text-align:center}
  .hero h1{font-size:clamp(1.9rem,4.4vw,3.1rem);line-height:1.18;margin-bottom:18px;font-weight:700}
  .hero p{font-size:1.08rem;max-width:640px;margin:0 auto 32px;opacity:.92}
  .btn{display:inline-block;padding:13px 30px;border-radius:var(--radius);font-weight:600;
    font-size:.95rem;transition:.2s;border:2px solid transparent;cursor:pointer}
  .btn-primary{background:var(--accent);color:#20170a}
  .btn-primary:hover{filter:brightness(1.08);transform:translateY(-2px)}
  .btn-ghost{border-color:rgba(255,255,255,.6);color:#fff;margin-left:10px}
  .btn-ghost:hover{background:rgba(255,255,255,.12)}

  /* ---------- SECCIONES ---------- */
  section{padding:78px 0}
  .soft{background:var(--bg-soft)}
  .head{text-align:center;max-width:660px;margin:0 auto 46px}
  .head h2{font-size:clamp(1.5rem,3vw,2.1rem);margin-bottom:12px}
  .head p{color:var(--muted)}
  .eyebrow{display:inline-block;font-size:.75rem;font-weight:700;letter-spacing:2px;
    text-transform:uppercase;color:var(--brand-2);margin-bottom:10px}

  .grid{display:grid;gap:24px;grid-template-columns:repeat(auto-fit,minmax(250px,1fr))}
  .card{background:#fff;border:1px solid var(--line);border-radius:var(--radius);padding:30px 26px;transition:.25s}
  .card:hover{transform:translateY(-4px);box-shadow:0 12px 28px rgba(10,77,104,.10);border-color:#cfe0e8}
  .ico{width:46px;height:46px;border-radius:10px;background:var(--bg-soft);color:var(--brand);
    display:grid;place-items:center;font-size:1.3rem;margin-bottom:16px}
  .card h3{font-size:1.08rem;margin-bottom:8px}
  .card p{color:var(--muted);font-size:.94rem}

  .two{display:grid;grid-template-columns:1fr 1fr;gap:52px;align-items:center}
  .two h2{font-size:clamp(1.5rem,3vw,2.1rem);margin-bottom:16px}
  .two p{color:var(--muted);margin-bottom:14px}
  .stats{display:flex;gap:36px;margin-top:26px;flex-wrap:wrap}
  .stats b{display:block;font-size:1.9rem;color:var(--brand);line-height:1.1}
  .stats span{font-size:.85rem;color:var(--muted)}
  .media{aspect-ratio:4/3;border-radius:var(--radius);
    background:linear-gradient(135deg,#dbe8ee,#b9d3de);display:grid;place-items:center;
    color:var(--brand);font-size:.85rem;letter-spacing:1px;border:1px solid var(--line);text-align:center;padding:20px}

  /* ---------- CONTACTO ---------- */
  .contact{display:grid;grid-template-columns:1fr 1.1fr;gap:44px}
  .info li{list-style:none;display:flex;gap:12px;margin-bottom:18px;font-size:.95rem}
  .info li b{display:block;font-size:.78rem;text-transform:uppercase;letter-spacing:1px;color:var(--brand-2)}
  .info li span{color:var(--muted)}
  form{background:#fff;border:1px solid var(--line);border-radius:var(--radius);padding:28px}
  .field{margin-bottom:16px}
  label{display:block;font-size:.82rem;font-weight:600;margin-bottom:6px}
  input,textarea,select{width:100%;padding:11px 13px;border:1px solid var(--line);border-radius:8px;
    font:inherit;font-size:.94rem;background:#fff;color:var(--ink)}
  input:focus,textarea:focus,select:focus{outline:2px solid var(--brand-2);outline-offset:1px;border-color:transparent}
  textarea{min-height:110px;resize:vertical}
  form .btn-primary{width:100%;border:0}
  .note{font-size:.8rem;color:var(--muted);margin-top:12px;text-align:center}

  /* ---------- FOOTER ---------- */
  footer{background:var(--ink);color:#c8d3da;padding:44px 0 26px;font-size:.9rem}
  .fgrid{display:flex;justify-content:space-between;gap:26px;flex-wrap:wrap;margin-bottom:26px;align-items:center}
  footer .logo{color:#fff}
  footer .logo small{color:#8fa3ae}
  .fnav{display:flex;gap:22px;flex-wrap:wrap}
  .fnav a:hover{color:#fff}
  .copy{border-top:1px solid #2b3a45;padding-top:18px;text-align:center;font-size:.82rem;color:#8fa3ae}


  /* ---------- UBICACION / MAPA ---------- */
  .map{border:1px solid var(--line);border-radius:var(--radius);overflow:hidden;
    box-shadow:0 8px 24px rgba(10,77,104,.10);background:var(--bg-soft)}
  .map iframe{width:100%;height:420px;border:0;display:block}
  .map-actions{display:flex;gap:12px;justify-content:center;margin-top:24px;flex-wrap:wrap}
  .btn-outline{border-color:var(--brand);color:var(--brand);background:transparent}
  .btn-outline:hover{background:var(--brand);color:#fff}

  /* ---------- REDES SOCIALES ---------- */
  .social{display:flex;gap:10px;flex-wrap:wrap}
  .social a{width:40px;height:40px;border-radius:50%;display:grid;place-items:center;
    background:#fff;border:1px solid var(--line);color:var(--brand);transition:.22s}
  .social a svg{width:19px;height:19px;fill:currentColor}
  .social a:hover{transform:translateY(-3px);color:#fff}
  .social a.fb:hover{background:#1877f2;border-color:#1877f2}
  .social a.ig:hover{background:#d62976;border-color:#d62976}
  .social a.wa:hover{background:#25d366;border-color:#25d366}
  .social a.li:hover{background:#0a66c2;border-color:#0a66c2}
  .social a.xx:hover{background:#000000;border-color:#000000}
  footer .social a{background:transparent;border-color:#3a4a55;color:#c8d3da}

  /* ---------- BOTON SUBIR ---------- */
  #top{position:fixed;right:22px;bottom:22px;z-index:60;width:48px;height:48px;border:0;
    border-radius:50%;background:var(--brand);color:#fff;cursor:pointer;
    box-shadow:0 8px 20px rgba(0,0,0,.25);display:grid;place-items:center;
    opacity:0;visibility:hidden;transform:translateY(14px);transition:.25s}
  #top svg{width:20px;height:20px;fill:currentColor}
  #top.show{opacity:1;visibility:visible;transform:none}
  #top:hover{background:var(--accent);color:#20170a}

  /* ---------- RESPONSIVO ---------- */
  @media(max-width:860px){
    .two,.contact{grid-template-columns:1fr;gap:32px}
    .burger{display:block}
    nav{position:absolute;top:100%;left:0;right:0;background:#fff;border-bottom:1px solid var(--line);
      display:none;box-shadow:0 10px 20px rgba(0,0,0,.06)}
    nav.open{display:block}
    nav ul{flex-direction:column;gap:0;padding:8px 24px 18px}
    nav li{width:100%}
    nav a{display:block;padding:13px 0;border-bottom:1px solid var(--line)}
    .map iframe{height:300px}
    #top{right:14px;bottom:14px;width:44px;height:44px}
    .hero{padding:70px 0 64px}
    .btn-ghost{margin:12px 0 0}
  }
</style>
</head>
<body>

<!-- ==================== ENCABEZADO / HEADER ==================== -->
<header>
  <div class="bar">

    <!-- LOGO: para usar tu imagen, sustituye el <svg>...</svg> por:
         <img src="logo.png" alt="Logo" style="height:40px"> -->
    <a href="#inicio" class="logo" aria-label="Inicio">
      <svg viewBox="0 0 64 64" role="img" aria-hidden="true">
        <rect width="64" height="64" rx="14" fill="#0a4d68"/>
        <path d="M20 44V20h10.5c5.4 0 8.8 2.8 8.8 7.3 0 3.2-1.7 5.5-4.6 6.5l5.9 10.2h-6.4l-5-9.2h-3.3V44H20zm5.9-13.5h4.2c2.4 0 3.8-1.2 3.8-3.1s-1.4-3.1-3.8-3.1h-4.2v6.2z" fill="#ffffff"/>
        <circle cx="46" cy="24" r="4" fill="#f6a21d"/>
      </svg>
      <span>
        NOMBRE EMPRESA
        <small data-i18n="tagline">Soluciones profesionales</small>
      </span>
    </a>

    <!-- MENU: 4 opciones -->
    <nav id="nav">
      <ul>
        <li><a href="#inicio"    class="active" data-i18n="nav1">Inicio</a></li>
        <li><a href="#servicios"               data-i18n="nav2">Servicios</a></li>
        <li><a href="#nosotros"                data-i18n="nav3">Nosotros</a></li>
        <li><a href="#contacto"                data-i18n="nav4">Contacto</a></li>
      </ul>
    </nav>

    <div style="display:flex;align-items:center;gap:10px">
      <!-- SELECTOR DE IDIOMA -->
      <div class="lang" role="group" aria-label="Idioma / Language">
        <button id="btn-es" class="on" onclick="setLang('es')">ES</button>
        <button id="btn-en" onclick="setLang('en')">EN</button>
      </div>
      <button class="burger" onclick="document.getElementById('nav').classList.toggle('open')" aria-label="Menu">&#9776;</button>
    </div>

  </div>
</header>

<!-- ==================== INICIO / HOME ==================== -->
<section class="hero" id="inicio">
  <div class="wrap">
    <h1 data-i18n="heroTitle">Soluciones a la medida de tu empresa</h1>
    <p data-i18n="heroText">Diseñamos, implementamos y damos seguimiento a proyectos con estándares de calidad, tiempos claros y precios competitivos.</p>
    <a href="#contacto" class="btn btn-primary" data-i18n="heroBtn1">Solicitar cotización</a>
    <a href="#servicios" class="btn btn-ghost" data-i18n="heroBtn2">Ver servicios</a>
  </div>
</section>

<!-- ==================== SERVICIOS / SERVICES ==================== -->
<section id="servicios" class="soft">
  <div class="wrap">
    <div class="head">
      <span class="eyebrow" data-i18n="sv0">Servicios</span>
      <h2 data-i18n="svTitle">Lo que hacemos por ti</h2>
      <p data-i18n="svText">Un equipo, un solo responsable y resultados medibles en cada etapa del proyecto.</p>
    </div>
    <div class="grid">
      <article class="card">
        <div class="ico">&#9881;</div>
        <h3 data-i18n="s1t">Asesoría técnica</h3>
        <p data-i18n="s1p">Diagnóstico, alcance y recomendaciones claras antes de invertir un solo peso.</p>
      </article>
      <article class="card">
        <div class="ico">&#128736;</div>
        <h3 data-i18n="s2t">Implementación</h3>
        <p data-i18n="s2p">Ejecución con cronograma, entregables definidos y reportes de avance.</p>
      </article>
      <article class="card">
        <div class="ico">&#128202;</div>
        <h3 data-i18n="s3t">Mantenimiento</h3>
        <p data-i18n="s3p">Planes preventivos y correctivos para mantener todo operando sin sorpresas.</p>
      </article>
      <article class="card">
        <div class="ico">&#128172;</div>
        <h3 data-i18n="s4t">Soporte</h3>
        <p data-i18n="s4p">Atención directa por teléfono, correo o WhatsApp cuando lo necesites.</p>
      </article>
    </div>
  </div>
</section>

<!-- ==================== NOSOTROS / ABOUT ==================== -->
<section id="nosotros">
  <div class="wrap two">
    <div>
      <span class="eyebrow" data-i18n="ab0">Nosotros</span>
      <h2 data-i18n="abTitle">Experiencia que se nota en los resultados</h2>
      <p data-i18n="abP1">Somos una empresa mexicana enfocada en dar soluciones prácticas, con personal certificado y procesos documentados.</p>
      <p data-i18n="abP2">Trabajamos con transparencia: cotización detallada, tiempos reales y comunicación constante de principio a fin.</p>
      <div class="stats">
        <div><b>+15</b><span data-i18n="st1">Años de experiencia</span></div>
        <div><b>+200</b><span data-i18n="st2">Proyectos entregados</span></div>
        <div><b>98%</b><span data-i18n="st3">Clientes satisfechos</span></div>
      </div>
    </div>
    <!-- Sustituye por: <img src="foto.jpg" alt="Empresa"> -->
    <div class="media" data-i18n="imgAlt">IMAGEN / FOTO DE LA EMPRESA</div>
  </div>
</section>

<!-- ==================== CONTACTO / CONTACT ==================== -->
<section id="contacto" class="soft">
  <div class="wrap">
    <div class="head">
      <span class="eyebrow" data-i18n="ct0">Contacto</span>
      <h2 data-i18n="ctTitle">Solicita tu cotización</h2>
      <p data-i18n="ctText">Cuéntanos qué necesitas y te respondemos en menos de 24 horas hábiles.</p>
    </div>
    <div class="contact">
      <ul class="info">
        <li><span>&#128205;</span><div><b data-i18n="i1">Dirección</b><span>Calle Ejemplo 123, Col. Centro, Ciudad, México</span></div></li>
        <li><span>&#128222;</span><div><b data-i18n="i2">Teléfono</b><span>+52 (000) 000 0000</span></div></li>
        <li><span>&#9993;</span><div><b data-i18n="i3">Correo</b><span>contacto@empresa.com</span></div></li>
        <li><span>&#128336;</span><div><b data-i18n="i4">Horario</b><span data-i18n="i4v">Lunes a viernes, 9:00 a 18:00 h</span></div></li>
        <li><span>&#127760;</span><div><b data-i18n="i5">S&iacute;guenos</b>
          <div class="social" style="margin-top:8px">
        <a class="fb" href="https://facebook.com/" target="_blank" rel="noopener" aria-label="Facebook" title="Facebook">
          <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M13.5 21v-8h2.7l.4-3.1h-3.1V7.9c0-.9.25-1.5 1.55-1.5h1.65V3.7c-.29-.04-1.27-.13-2.4-.13-2.38 0-4.02 1.45-4.02 4.12v2.21H7.6V13h2.68v8h3.22z"/></svg></a>
        <a class="ig" href="https://instagram.com/" target="_blank" rel="noopener" aria-label="Instagram" title="Instagram">
          <svg viewBox="0 0 24 24" aria-hidden="true"><rect x="3" y="3" width="18" height="18" rx="5.2" fill="none" stroke="currentColor" stroke-width="2"/><circle cx="12" cy="12" r="4" fill="none" stroke="currentColor" stroke-width="2"/><circle cx="17.3" cy="6.7" r="1.35"/></svg></a>
        <a class="wa" href="https://wa.me/520000000000" target="_blank" rel="noopener" aria-label="WhatsApp" title="WhatsApp">
          <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M12 2.4a9.6 9.6 0 0 0-8.2 14.6L2.4 21.6l4.7-1.3A9.6 9.6 0 1 0 12 2.4z" fill="none" stroke="currentColor" stroke-width="1.9"/><path d="M9.3 8.2c.18-.42.37-.43.6-.44h.5c.17 0 .4 0 .58.45l.66 1.6c.1.25.03.46-.09.63l-.34.44c-.11.14-.2.29-.09.5.47.94 1.31 1.78 2.25 2.25.21.11.36.03.5-.09l.44-.35c.17-.12.38-.18.63-.08l1.6.66c.45.18.45.4.45.58v.5c-.01.23-.02.42-.44.6-.42.2-1.06.35-1.6.28-2.79-.36-5.02-2.59-5.38-5.38-.07-.54.08-1.18.28-1.6z"/></svg></a>
        <a class="li" href="https://linkedin.com/" target="_blank" rel="noopener" aria-label="LinkedIn" title="LinkedIn">
          <svg viewBox="0 0 24 24" aria-hidden="true"><circle cx="5" cy="4.6" r="2.4"/><rect x="3" y="9" width="4" height="12" rx="0.4"/><path d="M10 9h3.8v1.75h.05c.55-1 1.85-1.95 3.75-1.95 4 0 4.4 2.5 4.4 5.7V21h-4v-5.4c0-1.3-.02-3-1.85-3-1.86 0-2.15 1.42-2.15 2.9V21h-4V9z"/></svg></a>
        <a class="xx" href="https://x.com/" target="_blank" rel="noopener" aria-label="X" title="X">
          <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M17.6 3h3.2l-7 8 8.2 10h-6.4l-5-6.1L4.8 21H1.6l7.5-8.6L1.4 3h6.5l4.5 5.6L17.6 3z"/></svg></a>
          </div>
        </div></li>
      </ul>

      <form onsubmit="enviar(event)">
        <div class="field">
          <label for="n" data-i18n="f1">Nombre completo</label>
          <input id="n" name="nombre" required>
        </div>
        <div class="field">
          <label for="e" data-i18n="f2">Correo electrónico</label>
          <input id="e" name="correo" type="email" required>
        </div>
        <div class="field">
          <label for="t" data-i18n="f3">Teléfono</label>
          <input id="t" name="telefono" type="tel">
        </div>
        <div class="field">
          <label for="s" data-i18n="f4">Servicio de interés</label>
          <select id="s" name="servicio">
            <option data-i18n="o1">Asesoría técnica</option>
            <option data-i18n="o2">Implementación</option>
            <option data-i18n="o3">Mantenimiento</option>
            <option data-i18n="o4">Soporte</option>
          </select>
        </div>
        <div class="field">
          <label for="m" data-i18n="f5">Mensaje</label>
          <textarea id="m" name="mensaje" required></textarea>
        </div>
        <button type="submit" class="btn btn-primary" data-i18n="f6">Enviar solicitud</button>
        <p class="note" data-i18n="f7">Tus datos se usan únicamente para responder tu solicitud.</p>
      </form>
    </div>
  </div>
</section>


<!-- ==================== UBICACION / LOCATION ====================
     PARA CAMBIAR LA UBICACION:
     sustituye "Zocalo,Ciudad+de+Mexico" por la direccion real de la empresa
     en los TRES enlaces de abajo (usa + en lugar de espacios).
     Ejemplo: Av+Universidad+123,Villahermosa,Tabasco
     Tambien funciona con coordenadas: 17.9892,-92.9475
     No se necesita clave de Google (API key). -->
<section id="ubicacion">
  <div class="wrap">
    <div class="head">
      <span class="eyebrow" data-i18n="ub0">Ubicaci&oacute;n</span>
      <h2 data-i18n="ubTitle">D&oacute;nde estamos</h2>
      <p data-i18n="ubText">Vis&iacute;tanos en nuestras oficinas o ag&eacute;ndanos una cita previa.</p>
    </div>

    <div class="map">
      <iframe title="Google Maps"
        src="https://www.google.com/maps?q=Zocalo,Ciudad+de+Mexico&amp;hl=es&amp;z=15&amp;output=embed"
        loading="lazy" allowfullscreen referrerpolicy="no-referrer-when-downgrade"></iframe>
    </div>

    <div class="map-actions">
      <a class="btn btn-primary" target="_blank" rel="noopener" data-i18n="ubBtn1"
         href="https://www.google.com/maps/dir/?api=1&amp;destination=Zocalo,Ciudad+de+Mexico">C&oacute;mo llegar</a>
      <a class="btn btn-outline" target="_blank" rel="noopener" data-i18n="ubBtn2"
         href="https://www.google.com/maps/search/?api=1&amp;query=Zocalo,Ciudad+de+Mexico">Ver en Google Maps</a>
    </div>
  </div>
</section>
<!-- ==================== PIE / FOOTER ==================== -->
<footer>
  <div class="wrap">
    <div class="fgrid">
      <div class="logo">
        <svg viewBox="0 0 64 64" aria-hidden="true">
          <rect width="64" height="64" rx="14" fill="#0f7ea1"/>
          <path d="M20 44V20h10.5c5.4 0 8.8 2.8 8.8 7.3 0 3.2-1.7 5.5-4.6 6.5l5.9 10.2h-6.4l-5-9.2h-3.3V44H20zm5.9-13.5h4.2c2.4 0 3.8-1.2 3.8-3.1s-1.4-3.1-3.8-3.1h-4.2v6.2z" fill="#ffffff"/>
          <circle cx="46" cy="24" r="4" fill="#f6a21d"/>
        </svg>
        <span>NOMBRE EMPRESA<small data-i18n="tagline">Soluciones profesionales</small></span>
      </div>
      <div class="fnav">
        <a href="#inicio"    data-i18n="nav1">Inicio</a>
        <a href="#servicios" data-i18n="nav2">Servicios</a>
        <a href="#nosotros"  data-i18n="nav3">Nosotros</a>
        <a href="#contacto"  data-i18n="nav4">Contacto</a>
        <a href="#ubicacion" data-i18n="ub0">Ubicaci&oacute;n</a>
      </div>
      <div class="social">
        <a class="fb" href="https://facebook.com/" target="_blank" rel="noopener" aria-label="Facebook" title="Facebook">
          <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M13.5 21v-8h2.7l.4-3.1h-3.1V7.9c0-.9.25-1.5 1.55-1.5h1.65V3.7c-.29-.04-1.27-.13-2.4-.13-2.38 0-4.02 1.45-4.02 4.12v2.21H7.6V13h2.68v8h3.22z"/></svg></a>
        <a class="ig" href="https://instagram.com/" target="_blank" rel="noopener" aria-label="Instagram" title="Instagram">
          <svg viewBox="0 0 24 24" aria-hidden="true"><rect x="3" y="3" width="18" height="18" rx="5.2" fill="none" stroke="currentColor" stroke-width="2"/><circle cx="12" cy="12" r="4" fill="none" stroke="currentColor" stroke-width="2"/><circle cx="17.3" cy="6.7" r="1.35"/></svg></a>
        <a class="wa" href="https://wa.me/520000000000" target="_blank" rel="noopener" aria-label="WhatsApp" title="WhatsApp">
          <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M12 2.4a9.6 9.6 0 0 0-8.2 14.6L2.4 21.6l4.7-1.3A9.6 9.6 0 1 0 12 2.4z" fill="none" stroke="currentColor" stroke-width="1.9"/><path d="M9.3 8.2c.18-.42.37-.43.6-.44h.5c.17 0 .4 0 .58.45l.66 1.6c.1.25.03.46-.09.63l-.34.44c-.11.14-.2.29-.09.5.47.94 1.31 1.78 2.25 2.25.21.11.36.03.5-.09l.44-.35c.17-.12.38-.18.63-.08l1.6.66c.45.18.45.4.45.58v.5c-.01.23-.02.42-.44.6-.42.2-1.06.35-1.6.28-2.79-.36-5.02-2.59-5.38-5.38-.07-.54.08-1.18.28-1.6z"/></svg></a>
        <a class="li" href="https://linkedin.com/" target="_blank" rel="noopener" aria-label="LinkedIn" title="LinkedIn">
          <svg viewBox="0 0 24 24" aria-hidden="true"><circle cx="5" cy="4.6" r="2.4"/><rect x="3" y="9" width="4" height="12" rx="0.4"/><path d="M10 9h3.8v1.75h.05c.55-1 1.85-1.95 3.75-1.95 4 0 4.4 2.5 4.4 5.7V21h-4v-5.4c0-1.3-.02-3-1.85-3-1.86 0-2.15 1.42-2.15 2.9V21h-4V9z"/></svg></a>
        <a class="xx" href="https://x.com/" target="_blank" rel="noopener" aria-label="X" title="X">
          <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M17.6 3h3.2l-7 8 8.2 10h-6.4l-5-6.1L4.8 21H1.6l7.5-8.6L1.4 3h6.5l4.5 5.6L17.6 3z"/></svg></a>
      </div>
    </div>
    <div class="copy">&copy; <span id="year"></span> Nombre Empresa. <span data-i18n="rights">Todos los derechos reservados.</span></div>
  </div>
</footer>

<!-- ==================== BOTON SUBIR / BACK TO TOP ==================== -->
<button id="top" onclick="subir()" aria-label="Subir" title="Subir">
  <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M12 4l8 8h-5v8H9v-8H4l8-8z"/></svg>
</button>

<script>
/* ============ TEXTOS EN ESPANOL E INGLES ============
   Para cambiar un texto, editalo en los dos idiomas (es / en).
   El HTML usa data-i18n="clave" para saber que texto le toca. */
const T = {
  es:{
    tagline:"Soluciones profesionales",
    nav1:"Inicio", nav2:"Servicios", nav3:"Nosotros", nav4:"Contacto",
    heroTitle:"Soluciones a la medida de tu empresa",
    heroText:"Diseñamos, implementamos y damos seguimiento a proyectos con estándares de calidad, tiempos claros y precios competitivos.",
    heroBtn1:"Solicitar cotización", heroBtn2:"Ver servicios",
    sv0:"Servicios", svTitle:"Lo que hacemos por ti",
    svText:"Un equipo, un solo responsable y resultados medibles en cada etapa del proyecto.",
    s1t:"Asesoría técnica", s1p:"Diagnóstico, alcance y recomendaciones claras antes de invertir un solo peso.",
    s2t:"Implementación", s2p:"Ejecución con cronograma, entregables definidos y reportes de avance.",
    s3t:"Mantenimiento", s3p:"Planes preventivos y correctivos para mantener todo operando sin sorpresas.",
    s4t:"Soporte", s4p:"Atención directa por teléfono, correo o WhatsApp cuando lo necesites.",
    ab0:"Nosotros", abTitle:"Experiencia que se nota en los resultados",
    abP1:"Somos una empresa mexicana enfocada en dar soluciones prácticas, con personal certificado y procesos documentados.",
    abP2:"Trabajamos con transparencia: cotización detallada, tiempos reales y comunicación constante de principio a fin.",
    st1:"Años de experiencia", st2:"Proyectos entregados", st3:"Clientes satisfechos",
    imgAlt:"IMAGEN / FOTO DE LA EMPRESA",
    ct0:"Contacto", ctTitle:"Solicita tu cotización",
    ctText:"Cuéntanos qué necesitas y te respondemos en menos de 24 horas hábiles.",
    i1:"Dirección", i2:"Teléfono", i3:"Correo", i4:"Horario",
    i4v:"Lunes a viernes, 9:00 a 18:00 h",
    f1:"Nombre completo", f2:"Correo electrónico", f3:"Teléfono", f4:"Servicio de interés",
    f5:"Mensaje", f6:"Enviar solicitud", f7:"Tus datos se usan únicamente para responder tu solicitud.",
    o1:"Asesoría técnica", o2:"Implementación", o3:"Mantenimiento", o4:"Soporte",
    i5:"Síguenos",
    ub0:"Ubicación", ubTitle:"Dónde estamos",
    ubText:"Visítanos en nuestras oficinas o agéndanos una cita previa.",
    ubBtn1:"Cómo llegar", ubBtn2:"Ver en Google Maps",
    rights:"Todos los derechos reservados.",
    title:"Nombre Empresa | Soluciones profesionales",
    ok:"¡Gracias! Hemos recibido tu solicitud. Te contactaremos pronto."
  },
  en:{
    tagline:"Professional solutions",
    nav1:"Home", nav2:"Services", nav3:"About us", nav4:"Contact",
    heroTitle:"Solutions tailored to your business",
    heroText:"We design, implement and follow up on projects with quality standards, clear timelines and competitive pricing.",
    heroBtn1:"Request a quote", heroBtn2:"See services",
    sv0:"Services", svTitle:"What we do for you",
    svText:"One team, one point of contact and measurable results at every stage of the project.",
    s1t:"Technical consulting", s1p:"Assessment, scope and clear recommendations before you invest a single peso.",
    s2t:"Implementation", s2p:"Execution with a schedule, defined deliverables and progress reports.",
    s3t:"Maintenance", s3p:"Preventive and corrective plans to keep everything running without surprises.",
    s4t:"Support", s4p:"Direct assistance by phone, email or WhatsApp whenever you need it.",
    ab0:"About us", abTitle:"Experience you can see in the results",
    abP1:"We are a Mexican company focused on practical solutions, with certified staff and documented processes.",
    abP2:"We work transparently: detailed quotes, realistic timelines and constant communication from start to finish.",
    st1:"Years of experience", st2:"Projects delivered", st3:"Satisfied clients",
    imgAlt:"COMPANY IMAGE / PHOTO",
    ct0:"Contact", ctTitle:"Request your quote",
    ctText:"Tell us what you need and we will reply within 24 business hours.",
    i1:"Address", i2:"Phone", i3:"Email", i4:"Business hours",
    i4v:"Monday to Friday, 9:00 am to 6:00 pm",
    f1:"Full name", f2:"Email address", f3:"Phone", f4:"Service of interest",
    f5:"Message", f6:"Send request", f7:"Your data is used only to answer your request.",
    o1:"Technical consulting", o2:"Implementation", o3:"Maintenance", o4:"Support",
    i5:"Follow us",
    ub0:"Location", ubTitle:"Where we are",
    ubText:"Visit our offices or schedule an appointment in advance.",
    ubBtn1:"Get directions", ubBtn2:"View on Google Maps",
    rights:"All rights reserved.",
    title:"Company Name | Professional solutions",
    ok:"Thank you! We received your request and will contact you soon."
  }
};

let lang = localStorage.getItem("lang") || "es";

function setLang(l){
  lang = l;
  try{ localStorage.setItem("lang", l); }catch(e){}
  document.documentElement.lang = l;
  document.querySelectorAll("[data-i18n]").forEach(function(el){
    var k = el.getAttribute("data-i18n");
    if(T[l][k]) el.textContent = T[l][k];
  });
  document.getElementById("btn-es").classList.toggle("on", l === "es");
  document.getElementById("btn-en").classList.toggle("on", l === "en");
  document.title = T[l].title;
}

/* El formulario solo muestra un aviso. Para recibir los correos,
   usa un servicio como Formspree: <form action="https://formspree.io/f/TU_ID" method="POST">
   y borra el onsubmit="enviar(event)". */
function enviar(e){
  e.preventDefault();
  alert(T[lang].ok);
  e.target.reset();
}

/* Marca la opcion del menu segun la seccion visible */
var secs = document.querySelectorAll("section[id]");
var links = document.querySelectorAll("nav a");
var btnTop = document.getElementById("top");

window.addEventListener("scroll", function(){
  var cur = "";
  secs.forEach(function(s){ if(window.scrollY >= s.offsetTop - 120) cur = s.id; });
  if(cur === "ubicacion") cur = "contacto";   /* el mapa deja marcado Contacto */
  links.forEach(function(a){ a.classList.toggle("active", a.getAttribute("href") === "#" + cur); });

  /* el boton de subir aparece despues de 300 px */
  btnTop.classList.toggle("show", window.scrollY > 300);
});

function subir(){
  window.scrollTo({ top:0, behavior:"smooth" });
}

/* Cierra el menu movil al elegir una opcion */
links.forEach(function(a){
  a.addEventListener("click", function(){ document.getElementById("nav").classList.remove("open"); });
});

document.getElementById("year").textContent = new Date().getFullYear();
setLang(lang);
</script>
</body>
</html>
