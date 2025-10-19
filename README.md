<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Luis Cohen — Desarrollador Full Stack</title>
  <meta name="description" content="Portfolio de Luis Cohen: Full Stack, Python, R, C++, Java, Docker. Música, código y buena energía." />
  <meta property="og:title" content="Luis Cohen — Full Stack" />
  <meta property="og:description" content="👾 Programador por pasión, no por error de sintaxis. Full Stack | Python | R | C++ | Java | Docker." />
  <meta property="og:type" content="website" />
  <meta name="color-scheme" content="light dark" />
  <link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>👾</text></svg>">
  <style>
    :root{
      --bg:#0b0c10; --card:#12141a; --fg:#e6edf3; --muted:#9aa4ad; --accent:#6ee7b7; --accent-2:#8ab4f8;
      --ring:rgba(110,231,183,.3);
    }
    @media (prefers-color-scheme: light){
      :root{ --bg:#f6f8fa; --card:#ffffff; --fg:#0b1320; --muted:#5a6672; --accent:#0ea5e9; --accent-2:#7c3aed; --ring:rgba(14,165,233,.25); }
    }
    html,body{height:100%}
    body{
      margin:0; font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, "Helvetica Neue", Arial, "Noto Sans", "Apple Color Emoji","Segoe UI Emoji";
      background: radial-gradient(1200px 600px at 10% -10%, rgba(124,58,237,.10), transparent 60%),
                  radial-gradient(900px 500px at 110% 10%, rgba(14,165,233,.10), transparent 55%),
                  var(--bg);
      color:var(--fg);
      line-height:1.6;
    }
    .wrap{max-width:1000px; margin:0 auto; padding:28px 20px 64px;}
    header{
      display:flex; align-items:center; justify-content:space-between; gap:16px; padding:6px 0 8px;
      position:sticky; top:0; backdrop-filter: blur(10px); background: color-mix(in srgb, var(--bg) 80%, transparent);
      border-bottom:1px solid color-mix(in srgb, var(--fg) 12%, transparent);
      z-index:10;
    }
    nav a{
      color:var(--muted); text-decoration:none; margin-left:18px; font-weight:600; letter-spacing:.2px;
    }
    nav a:hover{ color:var(--fg) }
    .hero{
      display:grid; grid-template-columns: 1.2fr .8fr; gap:28px; align-items:center; margin-top:36px;
    }
    .card{
      background:linear-gradient(180deg, color-mix(in srgb, var(--card) 92%, transparent), var(--card));
      border:1px solid color-mix(in srgb, var(--fg) 10%, transparent);
      border-radius:20px; padding:24px; box-shadow: 0 10px 30px rgba(0,0,0,.15);
    }
    .pill{ display:inline-flex; align-items:center; gap:8px; font-size:12px; padding:6px 10px; border-radius:999px;
      border:1px solid color-mix(in srgb, var(--fg) 12%, transparent); color:var(--muted); background: color-mix(in srgb, var(--card) 92%, transparent);}
    h1{ font-size:clamp(28px, 5vw, 44px); line-height:1.15; margin:10px 0 4px;}
    .sub{ color:var(--muted); font-size:clamp(14px,2.1vw,18px); margin:6px 0 18px; }
    .actions{ display:flex; gap:12px; flex-wrap:wrap; margin-top:10px }
    .btn{
      appearance:none; border:0; cursor:pointer; font-weight:700; letter-spacing:.2px;
      padding:12px 16px; border-radius:12px; transition:transform .04s ease, box-shadow .2s ease;
      box-shadow: 0 6px 18px rgba(0,0,0,.15);
    }
    .btn-primary{ background:linear-gradient(180deg, var(--accent), color-mix(in srgb, var(--accent) 70%, black)); color:#051014 }
    .btn-ghost{ background:transparent; color:var(--fg); border:1px solid color-mix(in srgb, var(--fg) 18%, transparent) }
    .btn:active{ transform: translateY(1px) }
    .grid{ display:grid; grid-template-columns: repeat(2, 1fr); gap:20px; margin-top:20px;}
    .bio p{ margin:.4rem 0 }
    .stack{ display:flex; flex-wrap:wrap; gap:10px; margin-top:6px }
    .chip{
      border:1px solid color-mix(in srgb, var(--fg) 12%, transparent);
      padding:8px 10px; border-radius:12px; background: color-mix(in srgb, var(--card) 92%, transparent);
      display:inline-flex; align-items:center; gap:8px; font-weight:600;
    }
    .chip svg{ width:18px; height:18px }
    .section{ margin-top:44px }
    .section h2{ font-size:22px; margin:0 0 10px }
    footer{ margin-top:50px; color:var(--muted); font-size:14px; text-align:center }
    .kbd{font-family: ui-monospace, SFMono-Regular, Menlo, Consolas, "Liberation Mono", monospace; font-size:12px; padding:2px 6px; border-radius:6px;
      border:1px solid color-mix(in srgb, var(--fg) 18%, transparent); background: color-mix(in srgb, var(--card) 92%, transparent)}
    @media (max-width: 860px){
      .hero{ grid-template-columns: 1fr; }
      nav{display:none}
    }
    .ring{ outline: 2px solid var(--ring); outline-offset: 4px; border-radius: 16px }
    .projects{ display:grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap:16px }
    .project{ padding:18px; border-radius:16px; border:1px solid color-mix(in srgb, var(--fg) 12%, transparent);
      background: color-mix(in srgb, var(--card) 94%, transparent) }
    .project h3{ margin:4px 0 6px; font-size:18px }
    .project p{ margin:0; color:var(--muted) }
    a.link{ color: var(--accent-2); text-decoration: none; font-weight: 700 }
    a.link:hover{ text-decoration: underline }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="pill">👋 Hola, Soy <strong>Luis Cohen</strong></div>
      <nav>
        <a href="#sobre-mi">Sobre mí</a>
        <a href="#stack">Stack</a>
        <a href="#proyectos">Proyectos</a>
        <a href="#contacto">Contacto</a>
      </nav>
    </header>

    <main>
      <section class="hero">
        <div class="card ring">
          <div class="pill">🧩 Opción 4 — Divertida y cercana</div>
          <h1>Desarrollador Full Stack</h1>
          <p class="sub">
            👾 Programador por pasión, no por error de sintaxis.<br/>
            🧑‍💻 Frontend + Backend = Full Stack.<br/>
            🎸 Música, código y buena energía siempre.
          </p>
          <div class="actions">
            <a class="btn btn-primary" href="#proyectos">🚀 Ver proyectos</a>
            <a class="btn btn-ghost" href="#contacto">💬 Hablemos</a>
          </div>
        </div>

        <div class="card bio" id="sobre-mi">
          <h2>Sobre mí</h2>
          <p>Me gusta construir productos simples, rápidos y útiles. Disfruto el <span class="kbd">clean code</span>, la automatización y el aprendizaje continuo.</p>
          <p>Actualmente enfocado en <strong>Python</strong> y <strong>datos</strong>, sin dejar de lado <strong>frontend</strong> y <strong>backend</strong>.</p>
        </div>
      </section>

      <section class="section" id="stack">
        <h2>🛠️ Stack principal</h2>
        <div class="stack">
          <!-- Python -->
          <span class="chip" title="Python">
            <svg viewBox="0 0 128 128" aria-hidden="true"><path d="M63.4 1.6c-8.2 0-15 1.2-20.3 3.6-3.2 1.5-5.8 3.4-7.7 5.8-1.9 2.3-3.2 4.9-3.8 7.8-.6 2.8-.9 5.6-.9 8.4v15.2h41.3v5.1H21.1c-4.7 0-8.6 1.1-11.6 3.4-3 2.2-4.9 5.7-5.8 10.3-.9 4.6-1.3 10.1-1.3 16.4 0 6.2.5 11.5 1.6 15.8 1.1 4.3 2.8 7.6 5.2 9.9 2.4 2.3 5.4 3.8 9.2 4.5 3.8.7 8.3 1.1 13.5 1.1h8.9v-12.6c0-5.2 1.4-9.1 4.1-11.8 2.8-2.7 6.5-4 11.1-4h20.9c4.4 0 7.9-1.3 10.5-3.9 2.6-2.6 4.6-6.1 5.8-10.6 1.2-4.5 1.9-9.8 1.9-16.1 0-6.1-.5-11.2-1.5-15.4-1-4.2-2.6-7.4-4.8-9.6-2.2-2.2-5.1-3.7-8.6-4.5-3.5-.9-7.7-1.3-12.6-1.3H63.4z" fill="currentColor"/></svg>
            Python
          </span>
          <!-- R -->
          <span class="chip" title="R">
            <svg viewBox="0 0 128 128" aria-hidden="true"><ellipse cx="64" cy="64" rx="60" ry="42" fill="none" stroke="currentColor" stroke-width="10"/><path d="M48 80h20c18 0 28-8 28-20s-10-20-28-20H40v68" fill="none" stroke="currentColor" stroke-width="10"/></svg>
            R
          </span>
          <!-- C++ -->
          <span class="chip" title="C++">
            <svg viewBox="0 0 128 128" aria-hidden="true"><path d="M64 6l52 30v56L64 122 12 92V36L64 6z" fill="none" stroke="currentColor" stroke-width="10"/><text x="40" y="78" font-size="34" font-weight="700" fill="currentColor">C++</text></svg>
            C++
          </span>
          <!-- Java -->
          <span class="chip" title="Java">
            <svg viewBox="0 0 128 128" aria-hidden="true"><path d="M64 20c14 18-14 22 0 38-18-6-4-18 0-38zM30 96c22 10 46 10 68 0" fill="none" stroke="currentColor" stroke-width="8"/></svg>
            Java
          </span>
          <!-- Docker -->
          <span class="chip" title="Docker">
            <svg viewBox="0 0 128 128" aria-hidden="true"><rect x="16" y="64" width="24" height="18" rx="3" ry="3" stroke="currentColor" fill="none" stroke-width="6"/><rect x="44" y="64" width="24" height="18" rx="3" ry="3" stroke="currentColor" fill="none" stroke-width="6"/><rect x="72" y="64" width="24" height="18" rx="3" ry="3" stroke="currentColor" fill="none" stroke-width="6"/><path d="M12 90h100c0 10-10 20-30 20H42C24 110 12 100 12 90z" fill="none" stroke="currentColor" stroke-width="6"/></svg>
            Docker
          </span>
          <!-- etc -->
          <span class="chip" title="y más">✨ etc.</span>
        </div>
      </section>

      <section class="section" id="proyectos">
        <h2>📦 Proyectos destacados</h2>
        <div class="projects">
          <article class="project">
            <h3>🧠 Analítica con Python + R</h3>
            <p>Pipelines reproducibles, notebooks limpios y visualizaciones claras.</p>
            <p><a class="link" href="#" target="_blank" rel="noopener">Ver repo</a></p>
          </article>
          <article class="project">
            <h3>⚙️ API en Docker</h3>
            <p>Microservicio ligero con buenas prácticas de CI/CD y contenedores.</p>
            <p><a class="link" href="#" target="_blank" rel="noopener">Ver repo</a></p>
          </article>
          <article class="project">
            <h3>💻 C++ Performance</h3>
            <p>Ejemplos de estructuras de datos y optimización low-level.</p>
            <p><a class="link" href="#" target="_blank" rel="noopener">Ver repo</a></p>
          </article>
        </div>
      </section>

      <section class="section card" id="contacto">
        <h2>📬 Contacto</h2>
        <p>¿Colaboramos? Escríbeme o revisa mi código:</p>
        <div class="actions">
          <a class="btn btn-primary" href="https://github.com/" target="_blank" rel="noopener">⭐ GitHub</a>
          <a class="btn btn-ghost" href="mailto:luiscohen2014@gmail.com">✉️ Email</a>
          <a class="btn btn-ghost" href="https://www.linkedin.com/" target="_blank" rel="noopener">🔗 LinkedIn</a>
        </div>
      </section>

      <footer>
        Hecho con 💚 y buen café. — © <span id="yr"></span> Luis Cohen
      </footer>
    </main>
  </div>

  <script>
    // Año dinámico + scroll suave
    document.getElementById('yr').textContent = new Date().getFullYear();
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', e=>{
        const id = a.getAttribute('href');
        const el = document.querySelector(id);
        if(el){
          e.preventDefault();
          el.scrollIntoView({behavior:'smooth', block:'start'});
          history.pushState(null,'',id);
        }
      });
    });
  </script>
</body>
</html>
