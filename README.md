<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>ShadowMarket</title>

  <!-- FONT -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Inter', sans-serif;
    }

    body {
      background: radial-gradient(circle at top, #0f172a, #020617);
      color: #e5e7eb;
    }

    /* NAV */
    .nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 60px;
      background: rgba(0,0,0,0.6);
      backdrop-filter: blur(10px);
      position: sticky;
      top: 0;
      z-index: 10;
    }

    .logo {
      font-size: 24px;
      font-weight: 700;
    }

    .logo span {
      color: #22d3ee;
    }

    .nav a {
      margin-left: 30px;
      color: #cbd5f5;
      text-decoration: none;
      transition: 0.2s;
    }

    .nav a:hover {
      color: #22d3ee;
    }

    .login {
      color: #22d3ee;
    }

    /* HERO */
    .hero {
      text-align: center;
      padding: 120px 20px;
    }

    .hero h1 {
      font-size: 48px;
      margin-bottom: 15px;
    }

    .hero p {
      opacity: 0.8;
      margin-bottom: 30px;
    }

    .hero button {
      background: linear-gradient(135deg, #22d3ee, #6366f1);
      border: none;
      padding: 15px 35px;
      font-size: 16px;
      color: black;
      border-radius: 10px;
      cursor: pointer;
    }

    /* MARKET */
    .market {
      padding: 80px 60px;
    }

    .market h2 {
      margin-bottom: 40px;
      font-size: 32px;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
    }

    .card {
      background: rgba(255,255,255,0.05);
      border: 1px solid rgba(255,255,255,0.1);
      border-radius: 16px;
      padding: 25px;
      backdrop-filter: blur(8px);
      transition: 0.3s;
    }

    .card:hover {
      transform: translateY(-6px);
      border-color: #22d3ee;
      box-shadow: 0 0 25px rgba(34,211,238,0.3);
    }

    .card h3 {
      margin-bottom: 10px;
    }

    .card p {
      opacity: 0.8;
    }

    .card span {
      display: block;
      margin: 15px 0;
      font-size: 22px;
      color: #22d3ee;
    }

    .card button {
      width: 100%;
      padding: 10px;
      background: transparent;
      border: 1px solid #22d3ee;
      color: #22d3ee;
      border-radius: 8px;
      cursor: pointer;
      transition: 0.2s;
    }

    .card button:hover {
      background: #22d3ee;
      color: black;
    }

    /* TRUST */
    .trust {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px,1fr));
      padding: 80px 60px;
      gap: 40px;
      background: rgba(0,0,0,0.4);
      text-align: center;
    }

    .trust h3 {
      margin-bottom: 10px;
    }

    /* FOOTER */
    footer {
      text-align: center;
      padding: 30px;
      opacity: 0.6;
      font-size: 14px;
    }

    /* MOBILE */
    @media (max-width: 768px) {
      .nav {
        padding: 20px;
      }

      .hero h1 {
        font-size: 36px;
      }

      .market, .trust {
        padding: 60px 20px;
      }
    }
  </style>
</head>

<body>

<header class="nav">
  <div class="logo">Shadow<span>Market</span></div>
  <nav>
    <a href="#market">Marketplace</a>
    <a href="#">Sell</a>
    <a href="#">Support</a>
    <a href="#" class="login">Login</a>
  </nav>
</header>

<section class="hero">
  <h1>Buy & Sell Digital Accounts</h1>
  <p>Secure marketplace for game accounts, items, and digital services</p>
  <button onclick="document.getElementById('market').scrollIntoView({behavior:'smooth'})">
    Browse Marketplace
  </button>
</section>

<section class="market" id="market">
  <h2>Featured Listings</h2>

  <div class="grid">
    <div class="card">
      <h3>Valorant Account</h3>
      <p>Rank: Immortal · Full Access</p>
      <span>$120</span>
      <button>View Listing</button>
    </div>

    <div class="card">
      <h3>Fortnite Account</h3>
      <p>Rare OG Skins Included</p>
      <span>$95</span>
      <button>View Listing</button>
    </div>

    <div class="card">
      <h3>CS2 Prime</h3>
      <p>High Trust Factor</p>
      <span>$40</span>
      <button>View Listing</button>
    </div>

    <div class="card">
      <h3>GTA V Account</h3>
      <p>Modded · High Level</p>
      <span>$60</span>
      <button>View Listing</button>
    </div>
  </div>
</section>

<section class="trust">
  <div>
    <h3>🔒 Secure Trades</h3>
    <p>Buyer protection on every order</p>
  </div>
  <div>
    <h3>⚡ Instant Delivery</h3>
    <p>Fast automated delivery system</p>
  </div>
  <div>
    <h3>⭐ Verified Sellers</h3>
    <p>Trusted & reviewed community</p>
  </div>
</section>

<footer>
  © 2026 ShadowMarket · All rights reserved
</footer>

</body>
</html>
