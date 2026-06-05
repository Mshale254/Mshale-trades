<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>MSHALE TECH Trading Dashboard</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    background:#0f172a;
    color:white;
    font-family:Arial,sans-serif;
}

/* Header */

header{
    background:#1e293b;
    padding:10px 20px;
    box-shadow:0 2px 10px rgba(0,0,0,.4);
}

.logo-container{
    display:flex;
    align-items:center;
    justify-content:center;
    gap:15px;
}

.logo{
    width:55px;
    height:55px;
    border-radius:50%;
    object-fit:cover;
    border:2px solid #38bdf8;
}

.branding h1{
    color:#38bdf8;
    font-size:24px;
}

.branding p{
    color:#cbd5e1;
    font-size:13px;
}

/* Main Chart */

.chart-container{
    width:100%;
    height:calc(100vh - 90px);
}

#tradingview_chart{
    width:100%;
    height:100%;
}

/* Widgets */

.widget-section{
    padding:15px;
}

.widget-title{
    margin-bottom:10px;
    color:#38bdf8;
}

/* Floating Logo */

.floating-logo{
    position:fixed;
    right:20px;
    bottom:20px;
    z-index:9999;
}

.floating-logo img{
    width:50px;
    height:50px;
    border-radius:50%;
    border:2px solid #38bdf8;
    box-shadow:0 0 15px rgba(0,0,0,.6);
}

/* Footer */

.footer{
    background:#1e293b;
    text-align:center;
    padding:15px;
    color:#94a3b8;
}

@media(max-width:768px){

.logo-container{
    flex-direction:column;
}

.branding{
    text-align:center;
}

.chart-container{
    height:80vh;
}

}

</style>
</head>
<body>

<!-- HEADER -->

<header>

<div class="logo-container">

<img src="mshale-logo.jpg" alt="MSHALE TECH" class="logo">

<div class="branding">
<h1>MSHALE TECH</h1>
<p>Forex • Crypto • Stocks • Indices</p>
</div>

</div>

</header>

<!-- FULLSCREEN CHART -->

<div class="chart-container">

<div id="tradingview_chart"></div>

</div>

<!-- WATCHLIST -->

<div class="widget-section">

<h2 class="widget-title">Market Watchlist</h2>

<div class="tradingview-widget-container">
<div class="tradingview-widget-container__widget"></div>

<script type="text/javascript"
src="https://s3.tradingview.com/external-embedding/embed-widget-watchlist.js"
async>
{
  "colorTheme":"dark",
  "displayMode":"adaptive",
  "width":"100%",
  "height":500,
  "watchlist":[
    "FX:EURUSD",
    "OANDA:XAUUSD",
    "BINANCE:BTCUSDT",
    "NASDAQ:AAPL",
    "FOREXCOM:DJI",
    "BINANCE:ETHUSDT"
  ]
}
</script>

</div>

</div>

<!-- ECONOMIC CALENDAR -->

<div class="widget-section">

<h2 class="widget-title">Economic Calendar</h2>

<div class="tradingview-widget-container">
<div class="tradingview-widget-container__widget"></div>

<script type="text/javascript"
src="https://s3.tradingview.com/external-embedding/embed-widget-events.js"
async>
{
  "colorTheme":"dark",
  "isTransparent":false,
  "width":"100%",
  "height":600,
  "locale":"en",
  "importanceFilter":"-1,0,1"
}
</script>

</div>

</div>

<!-- FLOATING LOGO -->

<div class="floating-logo">

<img src="mshale-logo.jpg" alt="MSHALE TECH">

</div>

<!-- FOOTER -->

<div class="footer">

© 2026 MSHALE TECH | Professional Trading Dashboard

</div>

<!-- MAIN CHART -->

<script src="https://s3.tradingview.com/tv.js"></script>

<script>

new TradingView.widget({
    "autosize": true,
    "symbol": "BINANCE:BTCUSDT",
    "interval": "15",
    "timezone": "Africa/Nairobi",
    "theme": "dark",
    "style": "1",
    "locale": "en",
    "toolbar_bg": "#1e293b",
    "enable_publishing": false,
    "allow_symbol_change": true,
    "container_id": "tradingview_chart"
});

</script>

</body>
</html>.card p{color:var(--muted); font-size:14px; margin:0}

.pricing{display:grid; gap:16px}
@media (min-width:800px){ .pricing{grid-template-columns: repeat(5,1fr)} }
.price{background:linear-gradient(180deg, rgba(17,24,39,1), rgba(27,38,79,1)); border:1px solid rgba(255,255,255,.08); border-radius: var(--radius); padding:18px; box-shadow:var(--shadow)}
.price h4{margin:4px 0 6px; font-size:18px}
.price .amt{font-size:26px; font-weight:800}

.notice{margin-top:8px; font-size:14px; color:var(--muted)}

.footer{margin-top:48px; padding:26px 0 40px; border-top:1px solid rgba(255,255,255,.08); color:var(--muted)}
.badge{display:inline-flex; align-items:center; gap:8px; padding:10px 12px; border:1px dashed rgba(255,255,255,.18); border-radius:12px; color:var(--text)}

.tag{display:inline-flex; align-items:center; gap:8px; font-weight:700; color:var(--acc)}
.tag svg{opacity:.9}

  </style>
</head>
<body>
  <header class="container hero">
    <span class="pill">MSHALE TECH • Online Cyber Services</span>
    <h1><span class="grad">Stay Connected</span> & Get Your Digital Tasks Done Right</h1>
    <p>Fast, reliable help with common eCitizen & cyber services in Kenya — from HELB to KRA, SHIF, NSSF, passport, driving licence applications, and more. Chat us on WhatsApp to get started.</p>
    <div class="cta">
      <a class="btn primary" href="https://wa.me/254729829406" target="_blank" rel="noopener">Chat on WhatsApp</a>
      <a class="btn ghost" href="#services">View Services</a>
    </div>
  </header>  <main class="container">
    <!-- SERVICES -->
    <section id="services" class="section">
      <h2>Cyber Services</h2>
      <p class="sub">Legit, client‑authorized support only. We assist with official applications and profile updates.</p><div class="grid cols-3" style="margin-top:16px">
    <!-- Each card is a service -->
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>HELB – Change Payment Method</h3>
      <p>Switch between M‑Pesa ↔ Bank, or update bank details.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>HELB Profile Update (100%)</h3>
      <p>Complete and verify your portal profile.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>Inter‑Institutional Transfer</h3>
      <p>Guidance through the official process.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>HELB Application</h3>
      <p>New applications and support with required docs.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>KRA PIN Registration</h3>
      <p>Get your KRA PIN and iTax setup.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>SHA/SHIF Registration</h3>
      <p>Enroll and update dependants where applicable.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>NSSF Registration</h3>
      <p>Create or update your NSSF account.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>Police Clearance (Good Conduct)</h3>
      <p>Help booking and preparing for your eCitizen application.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>Driving Licence</h3>
      <p>New DL application & renewal assistance.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>TSC Number Application</h3>
      <p>Step‑by‑step guidance and document checklist.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>Passport Application</h3>
      <p>eCitizen form guidance and appointment booking.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>eTIMS Account Creation</h3>
      <p>Set up your eTIMS account correctly.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>CRB Clearance Guidance</h3>
      <p>Support to request your CRB status & clearance.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>Social Media Boosting</h3>
      <p>Panel/software setup & account management.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>Birth Certificate Application</h3>
      <p>Assist with online application & follow‑up.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>Document Assistance</h3>
      <p>Corrections & updates when officially authorized.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>Premium Apps (No Subscriptions)</h3>
      <p>One‑time setup for selected apps.</p>
    </article>
    <article class="card">
      <svg class="tick" width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><path d="M20 6L9 17l-5-5"/></svg>
      <h3>Marriage Certificate Application</h3>
      <p>Guidance on the application process.</p>
    </article>
  </div>
  <p class="notice">Note: First come, first served.</p>
</section>

<!-- VPN PACKAGES -->
<section class="section" id="vpn">
  <div class="tag" style="margin-bottom:8px">
    <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><path d="M2 12h20M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"/></svg>
    AIRTEL Unlimited – VPN Files Available
  </div>
  <h2>Stay Connected</h2>
  <p class="sub">HTTP Injector • HTTP Custom • Dark Tunnel • v2ray (EV2ray)</p>

  <div class="pricing" style="margin-top:16px">
    <div class="price"><h4>4 Days</h4><div class="amt">KSh 50</div></div>
    <div class="price"><h4>1 Week</h4><div class="amt">KSh 80</div></div>
    <div class="price"><h4>10 Days</h4><div class="amt">KSh 100</div></div>
    <div class="price"><h4>15 Days</h4><div class="amt">KSh 150</div></div>
    <div class="price"><h4>30 Days</h4><div class="amt">KSh 300</div></div>
  </div>

  <div class="cta" style="margin-top:18px">
    <a class="btn primary" href="https://wa.me/254729829406" target="_blank" rel="noopener">Order on WhatsApp</a>
    <a class="btn" href="#contact">See Contact</a>
  </div>
  <p class="notice">Powered by <strong>MSHALE‑TECH</strong> 🔥🤝✅♨️</p>
</section>

<!-- CONTACT -->
<section id="contact" class="section">
  <h2>Contact</h2>
  <p class="sub">Have a question? Message us and we’ll guide you through the right process.</p>
  <div class="cta" style="margin-top:12px">
    <a class="btn primary" href="https://wa.me/254729829406" target="_blank" rel="noopener">WhatsApp: +254 729 829 406</a>
    <a class="btn ghost" href="#services">Back to Services</a>
  </div>
</section>

  </main>  <footer class="container footer">
    <div class="badge">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M20 7l-8 10-5-5"/></svg>
      Legit, client‑authorized support only • © <span id="year"></span> Mshale Tech
    </div>
  </footer>  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script></body>
