# zone
 A modern football and Formula 1 news website with dark and light red-themed modes. Built using HTML, CSS, and JavaScript.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ZONE - Football & F1 News</title>
  <style>
    :root {
      --main-red: #e63946;
      --light-bg: #ffffff;
      --dark-bg: #1a1a1a;
      --light-text: #ffffff;
      --dark-text: #000000;
    }

    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: var(--light-bg);
      color: var(--dark-text);
      transition: all 0.3s ease;
    }

    header {
      background-color: var(--main-red);
      padding: 1rem;
      text-align: center;
      color: white;
    }

    nav a {
      color: white;
      margin: 0 1rem;
      text-decoration: none;
      font-weight: bold;
    }

    .container {
      padding: 1rem;
    }

    .news-section {
      margin-top: 2rem;
    }

    .news-section h2 {
      color: var(--main-red);
    }

    .social-links a {
      display: block;
      margin: 0.5rem 0;
      color: var(--main-red);
      text-decoration: none;
    }

    .dark-mode {
      background-color: var(--dark-bg);
      color: var(--light-text);
    }

    .dark-mode header {
      background-color: var(--main-red);
    }

    .toggle-btn {
      margin-top: 1rem;
      padding: 0.5rem 1rem;
      background-color: var(--main-red);
      color: white;
      border: none;
      cursor: pointer;
      border-radius: 5px;
    }
  </style>
</head>
<body>
  <header>
    <h1>ZONE</h1>
    <nav>
      <a href="#news">News</a>
      <a href="#social">Connect</a>
    </nav>
  </header>

  <div class="container">
    <button class="toggle-btn" onclick="toggleMode()">Toggle Dark/Light Mode</button>

    <section id="news" class="news-section">
      <h2>Latest Football & F1 News</h2>
      <ul>
        <li>⚽ Manchester City signs new striker ahead of Premier League season</li>
        <li>🏎️ Max Verstappen wins another thrilling Grand Prix</li>
        <li>⚽ Champions League group stage draw announced</li>
        <li>🏎️ Ferrari introduces major upgrades for upcoming races</li>
        <li>⚽ AFCON & EURO 2028 preparations in full swing</li>
      </ul>
    </section>

    <section id="social" class="social-links">
      <h2>Connect with Me</h2>
      <a href="https://www.facebook.com/yassin.sakr.838106" target="_blank">Facebook</a>
      <a href="https://www.instagram.com/yas_sinsakr" target="_blank">Instagram</a>
      <a href="https://www.threads.net/@yas_sinsakr" target="_blank">Threads</a>
      <a href="https://x.com/yassin78922" target="_blank">X (Twitter)</a>
      <a href="https://youtube.com/@zonezone-qbe" target="_blank">YouTube</a>
    </section>
  </div>

  <script>
    function toggleMode() {
      document.body.classList.toggle("dark-mode");
    }
  </script>
</body>
</html>
