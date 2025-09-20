<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>The Duke’s</title>
  <meta name="theme-color" content="#0d1b52" />
  <style>
    :root { --dukes: #0d1b52; }
    body {
      margin: 0;
      height: 100vh;
      background: var(--dukes);
      display: flex;
      align-items: center;   /* Centrage vertical */
      justify-content: center; /* Centrage horizontal */
      flex-direction: column;
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif;
      color: #fff;
    }
    .logo {
      max-width: 320px;   /* taille max */
      width: 70vw;        /* responsive */
      height: auto;
      display: block;
      filter: drop-shadow(0 6px 18px rgba(0,0,0,.4));
      animation: fadein 800ms ease-out both;
    }
    .hint {
      margin-top: 18px;
      font-size: 16px;
      opacity: .85;
    }
    @keyframes fadein {
      from { opacity: 0; transform: scale(0.95); }
      to   { opacity: 1; transform: scale(1); }
    }
  </style>
  <script>
    // Réglages
    const REDIRECT_TO = "./menu.pdf#view=FitH"; // chemin vers la carte
    const DELAY_MS = 2500; // délai (2,5s)

    window.addEventListener("load", () => {
      setTimeout(() => { window.location.href = REDIRECT_TO }, DELAY_MS);
    });
  </script>
</head>
<body>
  <img src="./logo.png" class="logo" alt="The Duke’s" />
  <div class="hint">Chargement du menu…</div>

  <noscript>
    <meta http-equiv="refresh" content="0; url=./menu.pdf#view=FitH" />
  </noscript>
</body>
</html>

