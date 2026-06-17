```html
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Coupe du Monde - Live</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="refresh" content="900">
  <style>
    * { box-sizing: border-box; }
    body {
      margin: 0;
      width: 100vw;
      height: 100vh;
      overflow: hidden;
      font-family: Arial, Helvetica, sans-serif;
      background: radial-gradient(circle at top, #12345f 0%, #07111f 45%, #02060d 100%);
      color: white;
    }
    header {
      height: 110px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0 55px;
      border-bottom: 1px solid rgba(255,255,255,0.15);
      background: rgba(0,0,0,0.35);
    }
    .title {
      font-size: 42px;
      font-weight: 800;
      letter-spacing: 1px;
    }
    .subtitle {
      font-size: 20px;
      color: #b9d7ff;
      margin-top: 6px;
    }
    .clock {
      text-align: right;
      font-size: 30px;
      font-weight: bold;
    }
    .date {
      font-size: 18px;
      color: #b9d7ff;
      margin-top: 6px;
    }
    main {
      height: calc(100vh - 110px);
      padding: 28px 42px 36px;
      display: grid;
      grid-template-columns: 1.2fr 1fr;
      grid-template-rows: 1fr 1fr;
      gap: 24px;
    }
    .card {
      background: rgba(255,255,255,0.08);
      border: 1px solid rgba(255,255,255,0.16);
      border-radius: 26px;
      box-shadow: 0 20px 50px rgba(0,0,0,0.35);
      overflow: hidden;
      backdrop-filter: blur(8px);
    }
    .card.large {
      grid-row: span 2;
    }
    .card h2 {
      margin: 0;
      padding: 20px 26px;
      font-size: 28px;
      background: linear-gradient(90deg, #0c5cff, #00b7ff);
      color: white;
      letter-spacing: 0.5px;
    }
    iframe {
      width: 100%;
      height: calc(100% - 72px);
      border: 0;
      background: white;
    }
    .footer {
      position: fixed;
      bottom: 8px;
      right: 20px;
      font-size: 13px;
      color: rgba(255,255,255,0.45);
    }
  </style>
</head>
<body>

<header>
  <div>
    <div class="title">🏆 COUPE DU MONDE FIFA</div>
    <div class="subtitle">Scores en direct • Prochains matchs • Classements</div>
  </div>
  <div>
    <div class="clock" id="clock">--:--</div>
    <div class="date" id="date">Chargement...</div>
  </div>
</header>

<main>
  <section class="card large">
    <h2>⚽ Scores & matchs à venir</h2>
    <iframe src="https://www.sportbusy.com/embed/world-cup" allowfullscreen></iframe>
  </section>

  <section class="card">
    <h2>📅 Programme</h2>
    <iframe src="https://www.sportbusy.com/embed/world-cup" allowfullscreen></iframe>
  </section>

  <section class="card">
    <h2>📊 Classements</h2>
    <iframe src="https://www.sportbusy.com/embed/world-cup" allowfullscreen></iframe>
  </section>
</main>

<div class="footer">Actualisation automatique toutes les 15 minutes</div>

<script>
  function updateClock() {
    const now = new Date();
    document.getElementById("clock").textContent =
      now.toLocaleTimeString("fr-FR", { hour: "2-digit", minute: "2-digit" });

    document.getElementById("date").textContent =
      now.toLocaleDateString("fr-FR", {
        weekday: "long",
        day: "2-digit",
        month: "long",
        year: "numeric"
      });
  }

  updateClock();
  setInterval(updateClock, 1000);
</script>

</body>
</html>
```
