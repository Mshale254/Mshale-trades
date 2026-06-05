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
</html>
