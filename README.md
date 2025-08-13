<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>PURRKET — To the Moon and Beyond!</title>
  <meta name="description" content="Purrket: o hub meme-friendly para lançar e crescer sua memecoin. Templates, IA e hype com transparência.">

  <!-- Fonte -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;800&display=swap" rel="stylesheet">

  <style>
    :root{
      --bg:#0b1b2b;        /* fundo espacial */
      --txt:#ffffff;       /* branco */
      --muted:#d6e0ea;     /* texto secundário */
      --cta:#f59e0b;       /* laranja dos botões */
      --border:#2a3a4b;    /* linhas sutis */
    }
    *{ box-sizing:border-box }
    html,body{ height:100% }
    body{
      margin:0; color:var(--txt); background:var(--bg);
      font-family:Poppins, ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, "Helvetica Neue", Arial;
      -webkit-font-smoothing:antialiased; -moz-osx-font-smoothing:grayscale;
    }

    /* Fundo com estrelas + brilho radial */
    .space-bg{
      position:fixed; inset:0; z-index:-1;
      background:
        radial-gradient(ellipse at center, rgba(255,196,0,.06), transparent 60%),
        radial-gradient(#fff 1px, transparent 1px);
      background-size:auto, 24px 24px;
      opacity:.22; pointer-events:none;
    }

    .container{ max-width:1200px; margin:0 auto; padding:0 20px }

    /* Navbar */
    header{
      position:sticky; top:0; z-index:40;
      background:rgba(11,27,43,.8); backdrop-filter: blur(10px);
      border-bottom:1px solid var(--border);
    }
    .nav{ display:flex; align-items:center; justify-content:space-between; padding:14px 0 }
    .brand{ display:flex; align-items:center; gap:12px; font-weight:800; font-size:20px }
    .brand-badge{ width:32px; height:32px; border-radius:12px; background:#facc15 }
    .links{ display:none; gap:28px; color:#e8eef5b3; font-weight:600 }
    .links a{ color:inherit; text-decoration:none }
    .links a:hover{ color:#fff }

    /* Hero */
    .hero{ padding:80px 0 }
    .grid{ display:grid; gap:40px; align-items:center }
    @media (min-width: 992px){ .grid{ grid-template-columns:1.1fr .9fr } }

    h1{ margin:0; line-height:1.05 }
    .kicker{ font-size:56px; font-weight:800 }
    @media (min-width:768px){ .kicker{ font-size:72px } }
    .headline{ margin-top:8px; font-size:44px; font-weight:800; color:#e9f0f7 }
    @media (min-width:768px){ .headline{ font-size:60px } }

    p.lead{ margin:18px 0 0; color:var(--muted); max-width:640px }

    .cta{ display:flex; flex-wrap:wrap; gap:14px; margin-top:28px }
    .btn{
      display:inline-flex; align-items:center; justify-content:center;
      padding:14px 22px; border-radius:16px; font-weight:700; text-decoration:none;
      transition:filter .2s ease, transform .05s ease, box-shadow .2s ease;
      will-change: filter, transform;
    }
    .btn:active{ transform:translateY(1px) }
    .btn-primary{ background:var(--cta); color:#111; box-shadow:0 8px 24px rgba(245,158,11,.25) }
    .btn-primary:hover{ filter:brightness(1.08) }
    .btn-ghost{ border:1px solid #ffffff44; color:#fff }
    .btn-ghost:hover{ border-color:#ffffff88 }

    /* Imagem do gato + brilho */
    .hero-visual{ position:relative; display:flex; justify-content:center }
    .glow{
      position:absolute; inset:-40px; border-radius:999px;
      filter:blur(60px); background:rgba(255,200,0,.12);
    }
    .cat{
      position:relative; width:min(560px, 92vw); height:auto; object-fit:contain;
      filter: drop-shadow(0 20px 60px rgba(0,0,0,.45));
    }

    /* Footer */
    footer{ border-top:1px solid var(--border); margin-top:40px }
    .foot{
      display:flex; gap:16px; justify-content:space-between;
      padding:16px 0; color:#cbd5e1a6; font-size:14px
    }
    .foot a{ color:inherit; text-decoration:none }

    @media (min-width:900px){ .links{ display:flex } }
  </style>
</head>
<body>
  <div class="space-bg" aria-hidden="true"></div>

  <!-- NAVBAR -->
  <header>
    <div class="container nav">
      <div class="brand">
        <div class="brand-badge" aria-hidden="true"></div>
        <span>Purrket</span>
      </div>
      <nav class="links" aria-label="Primary">
        <a href="#about">ABOUT</a>
        <a href="#how">HOW TO BUY</a>
        <a href="#roadmap">ROADMAP</a>
        <a href="#contact">CONTACT</a>
      </nav>
    </div>
  </header>

  <!-- HERO -->
  <main class="hero">
    <div class="container grid">
      <!-- Texto -->
      <div>
        <h1>
          <span class="kicker">PURRKET</span>
          <span class="headline">To the Moon<br>and Beyond!</span>
        </h1>
        <p class="lead">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed diam nonummy nibh ullamcorper tincidunt.
        </p>
        <div class="cta">
          <a href="#buy" class="btn btn-primary">BUY NOW</a>
          <a href="#chart" class="btn btn-ghost">CHART</a>
        </div>
      </div>

      <!-- Visual do gato -->
      <div class="hero-visual">
        <div class="glow" aria-hidden="true"></div>
        <img
          class="cat"
          alt="Purrket — gato astronauta realista"
          src="https://raw.githubusercontent.com/purrket-coder/purrket/bb9cecc0fbb63933669fdd1fd57e0cd239b73ab7/3dca68f3-a51a-44c7-97e2-3cc274e3bde1.png"
        />
      </div>
    </div>
  </main>

  <!-- FOOTER -->
  <footer>
    <div class="container foot">
      <div>© <span id="y"></span> Purrket. All rights reserved.</div>
      <div><a href="#">Terms</a> · <a href="#">Privacy</a> · <a href="#">Contact</a></div>
    </div>
  </footer>

  <script>
    // ano atual no rodapé
    document.getElementById('y').textContent = new Date().getFullYear();
  </script>
</body>
</html>

