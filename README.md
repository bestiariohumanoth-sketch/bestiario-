<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Bestiario Humano — Agencia de Talento para Ficción</title>
  <meta name="description" content="Bestiario Humano: agencia de talento humano para ficción (fantasía, terror y ciencia ficción)." />
  <style>
    :root{
      --bg:#0b0b0f;
      --panel:#11111a;
      --text:#f2f2f5;
      --muted:#b8b8c5;
      --line:rgba(255,255,255,.12);
      --accent:#ffffff;
      --shadow:0 18px 40px rgba(0,0,0,.55);
      --radius:18px;
      --max:1100px;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Arial, "Apple Color Emoji","Segoe UI Emoji";
      background: radial-gradient(1200px 600px at 50% -10%, rgba(255,255,255,.10), transparent 60%),
                  radial-gradient(900px 600px at 0% 30%, rgba(255,255,255,.06), transparent 55%),
                  var(--bg);
      color:var(--text);
      line-height:1.55;
    }
    a{color:var(--accent); text-decoration:none}
    a:hover{text-decoration:underline}

    /* Layout */
    .wrap{max-width:var(--max); margin:0 auto; padding:24px}
    .nav{
      position:sticky; top:0; z-index:20;
      backdrop-filter: blur(10px);
      background: rgba(11,11,15,.72);
      border-bottom:1px solid var(--line);
    }
    .nav-inner{
      display:flex; align-items:center; justify-content:space-between;
      gap:16px;
      padding:14px 24px;
      max-width:var(--max);
      margin:0 auto;
    }
    .brand{
      display:flex; align-items:center; gap:12px;
      min-width: 220px;
    }
    .mark{
      width:38px; height:38px;
      border:1px solid var(--line);
      border-radius:12px;
      display:grid; place-items:center;
      box-shadow: var(--shadow);
      background: linear-gradient(180deg, rgba(255,255,255,.08), rgba(255,255,255,.02));
    }
    .brand h1{font-size:15px; margin:0; letter-spacing:.12em; text-transform:uppercase}
    .brand p{margin:2px 0 0; font-size:12px; color:var(--muted)}

    .links{display:flex; flex-wrap:wrap; gap:10px; justify-content:flex-end}
    .links a{
      font-size:13px; color:var(--muted);
      padding:8px 10px;
      border-radius:12px;
      border:1px solid transparent;
    }
    .links a:hover{color:var(--text); border-color:var(--line); text-decoration:none}

    /* Hero */
    .hero{
      padding:64px 0 34px;
    }
    .hero-grid{
      display:grid;
      grid-template-columns: 1.25fr .75fr;
      gap:18px;
      align-items:stretch;
    }
    @media (max-width: 900px){
      .hero-grid{grid-template-columns:1fr;}
      .brand{min-width:auto}
      .links{justify-content:flex-start}
    }

    .card{
      background: linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.02));
      border:1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
    }
    .hero-left{padding:28px}
    .kicker{color:var(--muted); font-size:12px; letter-spacing:.18em; text-transform:uppercase}
    .title{font-size:42px; margin:10px 0 10px; line-height:1.05}
    .subtitle{color:var(--muted); margin:0 0 18px; font-size:16px}

    .cta-row{display:flex; flex-wrap:wrap; gap:10px; margin-top:18px}
    .btn{
      display:inline-flex; align-items:center; justify-content:center;
      gap:10px;
      padding:12px 14px;
      border-radius: 14px;
      border:1px solid var(--line);
      background: rgba(0,0,0,.28);
      color:var(--text);
      font-weight:600;
      font-size:14px;
    }
    .btn.primary{
      background: rgba(255,255,255,.10);
      border-color: rgba(255,255,255,.22);
    }
    .btn:hover{transform: translateY(-1px); text-decoration:none}

    .hero-right{padding:22px}
    .stat{
      display:grid; gap:6px;
      padding:14px;
      border:1px dashed rgba(255,255,255,.18);
      border-radius: 16px;
      background: rgba(0,0,0,.18);
    }
    .stat strong{font-size:14px}
    .stat span{color:var(--muted); font-size:13px}
    .stack{display:grid; gap:12px}

    /* Sections */
    section{padding:26px 0}
    .section-title{font-size:18px; margin:0 0 10px; letter-spacing:.08em; text-transform:uppercase}
    .section-sub{margin:0 0 18px; color:var(--muted)}

    .grid-3{display:grid; grid-template-columns:repeat(3, 1fr); gap:14px}
    @media (max-width: 900px){.grid-3{grid-template-columns:1fr}}

    .panel{padding:18px}
    .panel h3{margin:0 0 8px; font-size:16px}
    .panel p{margin:0; color:var(--muted)}

    .divider{height:1px; background:var(--line); margin:22px 0}

    /* Contact */
    .contact{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap:14px;
      align-items:stretch;
    }
    @media (max-width: 900px){.contact{grid-template-columns:1fr}}

    .contact .panel p{color:var(--text)}
    .chip{
      display:inline-flex; align-items:center; gap:10px;
      padding:10px 12px;
      border-radius: 14px;
      border:1px solid var(--line);
      background: rgba(0,0,0,.20);
      font-weight:600;
    }

    footer{padding:24px 0 44px; color:var(--muted); font-size:13px}
    .tiny{font-size:12px; color:var(--muted)}

    /* Simple trident mark */
    svg{display:block}
  </style>
</head>
<body>
  <!-- NAV -->
  <div class="nav">
    <div class="nav-inner">
      <div class="brand" aria-label="Bestiario Humano">
        <div class="mark" aria-hidden="true">
          <!-- LOGO REAL: reemplaza el src por tu logo final en PNG/SVG -->
          <img src="logo-bestiario-humano.png" alt="Bestiario Humano" style="width:100%;height:100%;object-fit:contain" />
        </div>
        <div>
          <h1>Bestiario Humano</h1>
          <p>Agencia de Talento para Ficción</p>
        </div>
      </div>

      <nav class="links" aria-label="Navegación">
        <a href="#mision">Misión</a>
        <a href="#vision">Visión</a>
        <a href="#quienes">Quiénes somos</a>
        <a href="#contacto">Contacto</a>
      </nav>
    </div>
  </div>

  <main class="wrap">
    <!-- HERO -->
    <header class="hero" id="inicio">
      <div class="hero-grid">
        <div class="card hero-left">
          <div class="kicker">Talento humano • caracterización • ficción</div>
          <h2 class="title">Cuerpos reales para criaturas inolvidables.</h2>
          <p class="subtitle">
            Conectamos artistas, performers y modelos (todas las razas, edades, tallas y estéticas) con producciones de
            fantasía, terror y ciencia ficción. Casting ágil, portafolio curado y acompañamiento profesional.
          </p>

          <div class="cta-row">
            <a class="btn primary" href="#postulate">Postúlate</a>
            <a class="btn" href="#contacto">Hablar por WhatsApp</a>
            <a class="btn" href="mailto:bestiariohumanoth@gmail.com">Enviar email</a>
          </div>

          <div class="divider"></div>
          <p class="tiny">*Sitio base listo para personalizar con tus fotos, logo final y formulario de postulación.</p>
        </div>

        <aside class="card hero-right">
          <div class="stack">
            <div class="stat">
              <strong>Convocatoria Abierta</strong>
              <span>Artistas, performers y modelos para ficción.</span>
            </div>
            <div class="stat">
              <strong>Galería viva</strong>
              <span>Books de criaturas creados con aliados creativos.</span>
            </div>
            <div class="stat">
              <strong>Postúlate</strong>
              <span>Formulario rápido y claro.</span>
            </div>
          </div>
        </aside>
      </div>
    </header>

    <!-- MISIÓN / VISIÓN / QUIÉNES -->
    <section id="mision">
      <h2 class="section-title">Misión</h2>
      <p class="section-sub">
        Representar y proyectar talento humano diverso para la creación de personajes de ficción, conectándolo con
        productoras y proyectos creativos mediante un proceso ágil, transparente y profesional.
      </p>
      <div class="grid-3">
        <div class="card panel">
          <h3>Diversidad real</h3>
          <p>Razas, edades, cuerpos y estéticas: el casting que la ficción necesita.</p>
        </div>
        <div class="card panel">
          <h3>Curaduría & velocidad</h3>
          <p>Perfiles claros, búsqueda rápida y shortlist listo para decisión.</p>
        </div>
        <div class="card panel">
          <h3>Cuidado del talento</h3>
          <p>Comunicación, acuerdos claros, acompañamiento y respeto por el proceso.</p>
        </div>
      </div>
    </section>

    <section id="vision">
      <h2 class="section-title">Visión</h2>
      <p class="section-sub">
        Ser la agencia referente en Colombia para talento de caracterización y ficción, reconocida por su estética,
        su ética de trabajo y por impulsar colaboraciones que eleven el nivel del maquillaje, la fotografía y el
        performance en la industria.
      </p>
    </section>

    <section id="quienes">
      <h2 class="section-title">Quiénes somos</h2>
      <p class="section-sub">
        Bestiario Humano es una plataforma/agencia dedicada a representar talento para personajes de fantasía, terror y
        ciencia ficción. Trabajamos en alianza con artistas de maquillaje (FX/creativo), fotógrafos y equipos de arte
        para construir books potentes y conectar talento con oportunidades reales.
      </p>
      <div class="grid-3">
        <div class="card panel">
          <h3>Qué hacemos</h3>
          <p>Reclutamiento, registro, representación, difusión, negociación y coordinación de casting.</p>
        </div>
        <div class="card panel">
          <h3>Cómo trabajamos</h3>
          <p>Brief → selección → prueba/portafolio → confirmación → producción → entrega.</p>
        </div>
        <div class="card panel">
          <h3>Lo que buscamos</h3>
          <p>Talento comprometido, creativo y confiable; aliados que quieran crear industria.</p>
        </div>
      </div>
    </section>

    <!-- GALERÍA -->
    <section id="galeria">
      <h2 class="section-title">Galería</h2>
      <p class="section-sub">Selección de criaturas y caracterizaciones. (Reemplaza las imágenes por las tuyas)</p>
      <div class="grid-3">
        <div class="card panel"><img src="galeria-1.jpg" alt="Criatura 1" style="width:100%;border-radius:12px"></div>
        <div class="card panel"><img src="galeria-2.jpg" alt="Criatura 2" style="width:100%;border-radius:12px"></div>
        <div class="card panel"><img src="galeria-3.jpg" alt="Criatura 3" style="width:100%;border-radius:12px"></div>
      </div>
    </section>

    <!-- POSTÚLATE -->
    <section id="postulate">
      <h2 class="section-title">Postúlate</h2>
      <p class="section-sub">¿Quieres ser parte del Bestiario Humano? Completa el formulario.</p>
      <div class="card panel">
        <p>
          👉 <strong>Formulario de postulación:</strong><br />
          <a href="https://forms.gle/PEGA_AQUI_TU_FORMULARIO" target="_blank">Abrir formulario de postulación</a>
        </p>
        <p class="tiny">Puedes usar Google Forms o Typeform. Reemplaza el enlace por el definitivo.</p>
      </div>
    </section>

    <!-- CONTACTO -->
    <section id="contacto">
      <h2 class="section-title">Contacto</h2>
      <p class="section-sub">Hablemos de tu producción o de tu postulación para el Bestiario.</p>

      <div class="contact">
        <div class="card panel">
          <h3>WhatsApp</h3>
          <p style="margin:0 0 12px; color:var(--muted)">Respuesta rápida para castings, alianzas y dudas.</p>
          <a class="chip" href="https://wa.me/573165762498" target="_blank" rel="noopener">
            +57 316 576 2498
          </a>
        </div>

        <div class="card panel">
          <h3>Email</h3>
          <p style="margin:0 0 12px; color:var(--muted)">Envíanos el brief, fechas y referencias visuales.</p>
          <a class="chip" href="mailto:bestiariohumanoth@gmail.com">bestiariohumanoth@gmail.com</a>
        </div>
      </div>

      <div class="divider"></div>

      <div class="card panel">
        <h3>¿Eres talento o aliado creativo?</h3>
        <p>
          Escríbenos por WhatsApp con: nombre, ciudad, disponibilidad, 3 fotos recientes (rostro y cuerpo),
          y enlaces a portafolio/redes. Si eres fotógrafo/a o artista de maquillaje, comparte tu portafolio y
          propuesta de colaboración.
        </p>
      </div>
    </section>

    <footer>
      <div>© <span id="y"></span> Bestiario Humano — Agencia de Talento para Ficción</div>
      <div class="tiny">Hecho para crecer: agrega aquí tu formulario, galerías, catálogo de talento y casos de estudio.</div>
    </footer>
  </main>

  <script>
    document.getElementById('y').textContent = new Date().getFullYear();
  </script>
</body>
</html>
