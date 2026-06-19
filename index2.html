<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ГУ ДСНС Сумщина</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500;700;900&family=Rajdhani:wght@500;600;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" />
  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    body { font-family: 'Segoe UI', Arial, sans-serif; background: #0f172a; color: #e2e8f0; min-height: 100vh; }

    /* ===== ГОЛОВНА СТОРІНКА (ФОН НА ВСЮ СТОРІНКУ) ===== */
#page-home {
  position: relative;
  min-height: 100vh;
  display: flex; align-items: flex-start; justify-content: center;
  text-align: center; padding: 0;
  overflow: hidden;
}
#page-home .home-bg {
  position: absolute; inset: 0;
  background-image: url('dsns-1.jpeg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  filter: contrast(1) brightness(1) saturate(1);
  z-index: 0;
}
#page-home .home-overlay {
  position: absolute; inset: 0;
  background:
    linear-gradient(180deg, rgba(5,10,25,0.55) 0%, rgba(5,10,25,0) 22%, rgba(5,10,25,0) 70%, rgba(5,10,25,0.65) 100%);
  z-index: 1;
}
#page-home .home-content {
  position: relative; z-index: 2;
  width: 100%; max-width: 980px;
  padding: 48px 24px 0;
}
    }
    #page-home .home-eyebrow {
      font-family: 'Rajdhani', sans-serif;
      font-size: 12px; font-weight: 700; letter-spacing: 4px;
      color: #38bdf8; text-transform: uppercase;
      margin-bottom: 14px;
      text-shadow: 0 0 18px rgba(56,189,248,0.6);
    }
    #page-home .home-eyebrow::before,
    #page-home .home-eyebrow::after {
      content: '';
      display: inline-block; width: 36px; height: 1px;
      background: linear-gradient(90deg, transparent, #38bdf8);
      vertical-align: middle; margin: 0 10px 3px;
    }
    #page-home .home-eyebrow::after { background: linear-gradient(90deg, #38bdf8, transparent); }
    #page-home h1 {
      font-family: 'Orbitron', sans-serif;
      font-weight: 900;
      font-size: clamp(22px, 4.2vw, 44px);
      line-height: 1.25;
      letter-spacing: 1px;
      background: linear-gradient(135deg, #ffffff 0%, #93c5fd 45%, #38bdf8 75%, #818cf8 100%);
      -webkit-background-clip: text; background-clip: text; color: transparent;
      text-shadow: 0 4px 30px rgba(56,189,248,0.35);
      margin-bottom: 16px;
    }
    #page-home .home-divider {
      width: 110px; height: 3px; margin: 0 auto 18px;
      background: linear-gradient(90deg, transparent, #38bdf8, #818cf8, transparent);
      border-radius: 4px;
      box-shadow: 0 0 14px rgba(56,189,248,0.7);
    }
    #page-home p.home-sub {
      font-family: 'Rajdhani', sans-serif;
      font-weight: 600;
      font-size: clamp(13px, 1.6vw, 16px);
      letter-spacing: 0.4px;
      color: #cbd5e1;
    }
    #page-home p.home-hint {
      font-family: 'Rajdhani', sans-serif;
      font-weight: 500;
      font-size: 12px;
      letter-spacing: 0.5px;
      color: #64748b;
      margin-top: 26px;
    }

    /* ===== СТОРІНКА "ОПЕРАТИВНА ІНФОРМАЦІЯ" ===== */
    #page-operational { display: none; }
    #page-operational.active { display: block; }

    .dashboard-wrapper { max-width: 1600px; margin: 0 auto; padding: 0 8px 20px; }

    .main-header {
      display: flex; align-items: center; justify-content: space-between;
      background: #1e293b; border-bottom: 2px solid #2563eb;
      padding: 10px 14px; margin-bottom: 10px; border-radius: 0 0 8px 8px;
      flex-wrap: wrap; gap: 8px;
    }
    .header-logo-title { display: flex; align-items: center; gap: 10px; }
    .header-mini-logo { width: 40px; height: 40px; object-fit: contain; border-radius: 4px; }
    .main-header h1 { font-size: 13px; font-weight: 700; color: #f1f5f9; letter-spacing: 0.3px; line-height: 1.3; }
    .header-subtitle { font-size: 11px; color: #94a3b8; margin-top: 2px; }
    .date-badge {
      background: #0f172a; border: 1px solid #334155; border-radius: 6px;
      padding: 5px 10px; font-size: 12px; color: #38bdf8; font-family: monospace; font-weight: 600;
    }

    .top-counters-bar { display: grid; grid-template-columns: repeat(3, 1fr); gap: 6px; margin-bottom: 10px; }
    @media (min-width: 600px) { .top-counters-bar { grid-template-columns: repeat(6, 1fr); } }
    .counter-item {
      background: #1e293b; border-radius: 8px; border: 1px solid #334155;
      padding: 8px 6px; display: flex; flex-direction: column; align-items: center; gap: 3px;
    }
    .counter-label { font-size: 10px; color: #94a3b8; font-weight: 500; text-align: center; line-height: 1.2; }
    .counter-value { font-size: 22px; font-weight: 700; line-height: 1; }
    .fire-alert .counter-value     { color: #ef4444; }
    .accident-alert .counter-value { color: #f97316; }
    .bomb-alert .counter-value     { color: #eab308; }
    .shelling-alert .counter-value { color: #a78bfa; }
    .water-alert .counter-value    { color: #38bdf8; }
    .other-alert .counter-value    { color: #94a3b8; }

    .dashboard-grid { display: flex; flex-direction: column; gap: 10px; }
    @media (min-width: 700px)  { .dashboard-grid { display: grid; grid-template-columns: 1fr 1fr; } }
    @media (min-width: 1100px) { .dashboard-grid { grid-template-columns: repeat(3, 1fr); } }
    .grid-column { display: flex; flex-direction: column; gap: 10px; }

    .info-block { background: #1e293b; border-radius: 8px; border: 1px solid #334155; overflow: hidden; }
    .info-block h2 {
      font-size: 12px; font-weight: 600; color: #f1f5f9;
      padding: 8px 12px; border-bottom: 1px solid #334155; background: #0f172a; letter-spacing: 0.3px;
    }
    .info-block.blue-top h2 { border-left: 3px solid #2563eb; }
    .info-block.dark-top h2 { border-left: 3px solid #475569; }
    .padding-box { padding: 12px; }
    .points-list p { font-size: 12px; color: #cbd5e1; line-height: 1.6; margin-bottom: 8px; }
    .points-list p:last-child { margin-bottom: 0; }
    .dashed-line { border: none; border-top: 1px dashed #334155; margin: 8px 0; }

    .table-responsive-wrapper { overflow-x: auto; padding: 8px; -webkit-overflow-scrolling: touch; }
    .report-table { width: 100%; border-collapse: collapse; font-size: 11px; }
    .report-table th {
      background: #0f172a; color: #94a3b8; padding: 6px 8px; text-align: left;
      font-weight: 600; border-bottom: 1px solid #334155; font-size: 10px;
      text-transform: uppercase; letter-spacing: 0.4px; white-space: nowrap;
    }
    .report-table th.center, .report-table td.center { text-align: center; }
    .report-table td { padding: 5px 8px; border-bottom: 1px solid #1e293b; color: #cbd5e1; }
    .report-table tr:last-child td { border-bottom: none; }
    .highlight-row td { background: #0f172a; color: #f1f5f9; }
    .thick-row td { border-top: 2px solid #334155; }
    .border-double td { border-bottom: 2px solid #334155; }
    .indent-cell { padding-left: 18px !important; color: #94a3b8 !important; }
    .bold { font-weight: 600; }
    .alert-text { color: #ef4444 !important; font-weight: 700; }
    .text-orange { color: #f97316 !important; }
    .text-yellow { color: #eab308 !important; }
    .text-blue   { color: #38bdf8 !important; }
    .text-xs { font-size: 10px !important; }

    #sync-status {
      font-size: 10px; font-weight: normal; padding: 2px 6px;
      border-radius: 10px; margin-left: 6px; vertical-align: middle;
    }
    .sync-ok      { background: #14532d; color: #86efac; }
    .sync-loading { background: #713f12; color: #fde68a; }
    .sync-error   { background: #7f1d1d; color: #fca5a5; }

    #open-dsns-map { width: 100%; height: 320px; position: relative; }
    @media (min-width: 600px) { #open-dsns-map { height: 400px; } }
    @media (min-width: 1100px) { #open-dsns-map { height: 460px; } }

    .map-statusbar {
      position: absolute; top: 8px; left: 50%; transform: translateX(-50%);
      z-index: 1000; background: rgba(15,23,42,0.92); border: 1px solid #334155;
      border-radius: 20px; padding: 5px 12px;
      font-family: 'Segoe UI', Arial, sans-serif; font-size: 11px; color: #94a3b8;
      display: flex; gap: 8px; align-items: center; white-space: nowrap;
      max-width: calc(100% - 20px);
    }
    .dot-status { width: 7px; height: 7px; border-radius: 50%; background: #475569; flex-shrink: 0; }
    .dot-status.ok      { background: #22c55e; }
    .dot-status.loading { background: #eab308; animation: pulse 1s infinite; }
    @keyframes pulse { 0%,100%{opacity:1} 50%{opacity:.3} }

    .map-legend {
      position: absolute; bottom: 10px; right: 10px; z-index: 1000;
      background: rgba(15,23,42,0.92); border: 1px solid #334155;
      border-radius: 8px; padding: 8px 10px;
      font-family: 'Segoe UI', Arial, sans-serif; font-size: 11px; color: #cbd5e1;
    }
    .map-legend-title {
      font-weight: 700; font-size: 10px; text-transform: uppercase;
      letter-spacing: .05em; color: #94a3b8; margin-bottom: 6px;
    }
    .legend-item {
      display: flex; align-items: center; gap: 6px;
      margin-bottom: 4px; cursor: pointer; transition: opacity .2s;
      -webkit-tap-highlight-color: transparent;
    }
    .legend-item:last-child { margin-bottom: 0; }
    .legend-item.hidden-layer { opacity: .35; }

    .leaflet-popup-content-wrapper {
      background: #1e293b !important; border: 1px solid #475569 !important;
      border-radius: 8px !important; color: #e2e8f0 !important;
    }
    .leaflet-popup-tip { background: #1e293b !important; }
    .leaflet-popup-content { margin: 10px 12px !important; max-width: 220px; }
    .popup-layer  { font-size: 10px; font-weight: 700; text-transform: uppercase; margin-bottom: 4px; }
    .popup-desc   { font-size: 12px; color: #cbd5e1; line-height: 1.5; margin-bottom: 6px; }
    .popup-coords { font-size: 10px; color: #64748b; border-top: 1px solid #334155; padding-top: 4px; font-family: monospace; }

    .accordion-toggle {
      width: 100%; background: none; border: none; color: #94a3b8;
      font-size: 11px; padding: 6px 12px; text-align: right;
      cursor: pointer; display: flex; align-items: center; justify-content: flex-end; gap: 4px;
    }
    .accordion-toggle .arrow { transition: transform .2s; display: inline-block; }
    .accordion-toggle.open .arrow { transform: rotate(180deg); }
    .accordion-body { display: none; }
    .accordion-body.open { display: block; }

    /* ===== КНОПКА "НА ГОЛОВНУ" ===== */
    .back-home-btn {
      position: fixed; top: 14px; left: 14px; z-index: 1200;
      background: #1e293b; border: 1px solid #334155; border-radius: 8px;
      color: #e2e8f0; text-decoration: none; font-size: 13px;
      padding: 9px 14px; display: flex; align-items: center; gap: 6px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.4); transition: background .2s;
      cursor: pointer;
    }
    .back-home-btn:hover { background: #2563eb; border-color: #2563eb; }

    /* ===== BURGER + SIDEBAR ===== */
    .burger-btn {
      position: fixed; top: 14px; right: 14px; z-index: 1200;
      width: 40px; height: 40px; background: #1e293b;
      border: 1px solid #334155; border-radius: 8px;
      cursor: pointer; display: flex; flex-direction: column;
      align-items: center; justify-content: center; gap: 5px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.4);
      transition: background .2s;
    }
    .burger-btn:hover { background: #2563eb; border-color: #2563eb; }
    .burger-btn span {
      display: block; width: 20px; height: 2px;
      background: #e2e8f0; border-radius: 2px;
      transition: transform .3s, opacity .3s;
    }
    .burger-btn.open span:nth-child(1) { transform: translateY(7px) rotate(45deg); }
    .burger-btn.open span:nth-child(2) { opacity: 0; }
    .burger-btn.open span:nth-child(3) { transform: translateY(-7px) rotate(-45deg); }

    .sidebar-overlay {
      display: none; position: fixed; inset: 0; z-index: 1100;
      background: rgba(0,0,0,0.5); backdrop-filter: blur(2px);
    }
    .sidebar-overlay.active { display: block; }

    .sidebar {
      position: fixed; top: 0; right: -300px; width: 280px; height: 100%;
      z-index: 1150; background: #1e293b;
      border-left: 2px solid #2563eb;
      box-shadow: -4px 0 24px rgba(0,0,0,0.5);
      transition: right .35s cubic-bezier(.4,0,.2,1);
      display: flex; flex-direction: column; overflow: hidden;
    }
    .sidebar.open { right: 0; }

    .sidebar-header {
      padding: 16px 16px 12px;
      border-bottom: 1px solid #334155;
      background: #0f172a;
      flex-shrink: 0;
    }
    .sidebar-header h3 {
      font-size: 11px; font-weight: 700; color: #94a3b8;
      text-transform: uppercase; letter-spacing: 0.6px;
    }

    .sidebar-nav { flex: 1; overflow-y: auto; padding: 8px 0; }
    .sidebar-nav::-webkit-scrollbar { width: 4px; }
    .sidebar-nav::-webkit-scrollbar-track { background: #0f172a; }
    .sidebar-nav::-webkit-scrollbar-thumb { background: #334155; border-radius: 2px; }

    .sidebar-nav a {
      display: flex; align-items: center; gap: 10px;
      padding: 11px 16px; color: #cbd5e1; text-decoration: none;
      font-size: 13px; font-weight: 500; border-left: 3px solid transparent;
      transition: background .15s, border-color .15s, color .15s;
    }
    .sidebar-nav a:hover { background: #0f172a; border-left-color: #2563eb; color: #f1f5f9; }
    .sidebar-nav a .nav-num {
      font-size: 10px; color: #475569; font-family: monospace;
      min-width: 18px; text-align: right; flex-shrink: 0;
    }
    .sidebar-nav a .nav-icon { font-size: 16px; flex-shrink: 0; }
    .sidebar-nav .nav-divider {
      height: 1px; background: #334155; margin: 6px 16px;
    }
  
.pdf-btn{
  background:#dc2626;color:#fff;border:none;border-radius:6px;
  padding:6px 12px;cursor:pointer;font-size:12px;font-weight:600;
}
.pdf-btn:hover{background:#b91c1c;}

</style>

<script src="https://cdnjs.cloudflare.com/ajax/libs/html2canvas/1.4.1/html2canvas.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>

</head>
<body>

<!-- ===== ГОЛОВНА СТОРІНКА ===== -->
<section id="page-home">
  <div class="home-bg"></div>
  <div class="home-overlay"></div>
  <div class="home-content">
    <div class="home-eyebrow">ДСНС УКРАЇНИ</div>
    <h1>РЕГІОНАЛЬНИЙ ЦЕНТР УПРАВЛІННЯ<br>В НАДЗВИЧАЙНИХ СИТУАЦІЯХ</h1>
    <div class="home-divider"></div>
  </div>
</section>

<!-- ===== СТОРІНКА "ОПЕРАТИВНА ІНФОРМАЦІЯ" ===== -->
<section id="page-operational">

<!-- НА ГОЛОВНУ -->
<a href="#" class="back-home-btn" onclick="goHome(); return false;">← На головну</a>

<div class="dashboard-wrapper">

  <header class="main-header">
    <div class="header-logo-title">
      <img src="dsns-emblem.jpg" alt="ДСНС" class="header-mini-logo" onerror="this.style.display='none'">
      <div>
        <h1>ОПЕРАТИВНА ІНФОРМАЦІЯ ЗА ДОБУ</h1>
        <p class="header-subtitle">ГУ ДСНС України у Сумській області</p>
      </div>
    </div>
    <div class="header-meta" style="display:flex;align-items:center;gap:10px;">
      <span class="date-badge" id="dashboardClock">Завантаження...</span>
      <button class="pdf-btn" onclick="saveOperationalPDF()">📄 PDF</button>
    </div>
  </header>

  <section class="top-counters-bar">
    <div class="counter-item fire-alert">
      <span class="counter-label">🔥 Пожежі</span>
      <span class="counter-value" data-cell="C4">—</span>
    </div>
    <div class="counter-item accident-alert">
      <span class="counter-label">🚗 ДТП</span>
      <span class="counter-value" data-cell="C8">—</span>
    </div>
    <div class="counter-item bomb-alert">
      <span class="counter-label">💣 ВНП</span>
      <span class="counter-value" data-cell="C12">—</span>
    </div>
    <div class="counter-item shelling-alert">
      <span class="counter-label">🚀 Обстріли</span>
      <span class="counter-value" data-cell="G6">—</span>
    </div>
    <div class="counter-item water-alert">
      <span class="counter-label">🌊 Вода</span>
      <span class="counter-value" data-cell="C16">—</span>
    </div>
    <div class="counter-item other-alert">
      <span class="counter-label">⚠️ Інші</span>
      <span class="counter-value" data-cell="C20">—</span>
    </div>
  </section>

  <main class="dashboard-grid">

    <!-- КОЛОНКА 1 -->
    <div class="grid-column">
      <div class="info-block blue-top">
        <h2>🗺️ ОПЕРАТИВНА МАПА</h2>
        <div style="position:relative;">
          <div id="open-dsns-map"></div>
          <div class="map-statusbar">
            <div class="dot-status loading" id="map-status-dot"></div>
            <span id="map-status-text">Завантаження…</span>
          </div>
          <div class="map-legend" id="map-legend" style="display:none">
            <div class="map-legend-title">Шари</div>
            <div id="map-legend-items"></div>
          </div>
        </div>
      </div>

      <div class="info-block">
        <button class="accordion-toggle" onclick="toggleAccordion(this)">
          ⛺ Пункти незламності та обігріву <span class="arrow">▼</span>
        </button>
        <div class="accordion-body padding-box">
          <div class="points-list">
            <p><strong>Пункти незламності:</strong><br>
              Всього – 429, з них: Сумський р-н – 106, Конотопський р-н – 73, Охтирський р-н – 47, Роменський р-н – 29, Шосткинський р-н – 174.</p>
            <hr class="dashed-line">
            <p><strong>Пункти обігріву:</strong><br>
              Всього – 512, з них: Сумський р-н – 105, Конотопський р-н – 148, Охтирський р-н – 64, Роменський р-н – 88, Шосткинський р-н – 107.</p>
          </div>
        </div>
      </div>
    </div>

    <!-- КОЛОНКА 2 -->
    <div class="grid-column">
      <div class="info-block dark-top">
        <h2>📊 Події за напрямками <span id="sync-status"></span></h2>
        <div class="table-responsive-wrapper">
          <table class="report-table">
            <thead>
              <tr><th>Подій</th><th class="center">Доба</th><th class="center">Рік</th></tr>
            </thead>
            <tbody>
              <tr class="highlight-row"><td>Пожеж 🔥</td><td class="center bold alert-text" data-cell="C4">—</td><td class="center bold" data-cell="D4">—</td></tr>
              <tr><td class="indent-cell">Загиблі</td><td class="center" data-cell="C5">—</td><td class="center" data-cell="D5">—</td></tr>
              <tr><td class="indent-cell">Травмовані</td><td class="center" data-cell="C6">—</td><td class="center" data-cell="D6">—</td></tr>
              <tr><td class="indent-cell">Врятовані</td><td class="center" data-cell="C7">—</td><td class="center" data-cell="D7">—</td></tr>
              <tr class="highlight-row"><td>ДТП 🚗</td><td class="center bold text-orange" data-cell="C8">—</td><td class="center bold" data-cell="D8">—</td></tr>
              <tr><td class="indent-cell">Загиблі</td><td class="center" data-cell="C9">—</td><td class="center" data-cell="D9">—</td></tr>
              <tr><td class="indent-cell">Травмовані</td><td class="center" data-cell="C10">—</td><td class="center" data-cell="D10">—</td></tr>
              <tr><td class="indent-cell">Врятовані</td><td class="center" data-cell="C11">—</td><td class="center" data-cell="D11">—</td></tr>
              <tr class="highlight-row"><td>ВНП 💣</td><td class="center bold text-yellow" data-cell="C12">—</td><td class="center bold" data-cell="D12">—</td></tr>
              <tr><td class="indent-cell">Виявлено</td><td class="center" data-cell="C13">—</td><td class="center" data-cell="D13">—</td></tr>
              <tr><td class="indent-cell">Знищено</td><td class="center" data-cell="C14">—</td><td class="center" data-cell="D14">—</td></tr>
              <tr><td class="indent-cell">Одиниці</td><td class="center" data-cell="C15">—</td><td class="center" data-cell="D15">—</td></tr>
              <tr class="highlight-row"><td>НП на воді 🌊</td><td class="center bold text-blue" data-cell="C16">—</td><td class="center bold" data-cell="D16">—</td></tr>
              <tr><td class="indent-cell">Загиблі</td><td class="center" data-cell="C17">—</td><td class="center" data-cell="D17">—</td></tr>
              <tr><td class="indent-cell">Травмовані</td><td class="center" data-cell="C18">—</td><td class="center" data-cell="D18">—</td></tr>
              <tr><td class="indent-cell">Врятовані</td><td class="center" data-cell="C19">—</td><td class="center" data-cell="D19">—</td></tr>
              <tr class="highlight-row"><td>Інші НП ⚠️</td><td class="center bold" data-cell="C20">—</td><td class="center bold" data-cell="D20">—</td></tr>
              <tr><td class="indent-cell">Загиблі</td><td class="center" data-cell="C21">—</td><td class="center" data-cell="D21">—</td></tr>
              <tr><td class="indent-cell">Травмовані</td><td class="center" data-cell="C22">—</td><td class="center" data-cell="D22">—</td></tr>
              <tr class="highlight-row"><td>Врятовані (інші НП)</td><td class="center bold" data-cell="C23">—</td><td class="center bold" data-cell="D23">—</td></tr>
            </tbody>
          </table>
        </div>
      </div>

      <div class="info-block dark-top">
        <h2>🌱 Пожежі в екосистемах</h2>
        <div class="table-responsive-wrapper">
          <table class="report-table">
            <thead>
              <tr><th>Період</th><th class="center text-xs">Відкриті</th><th class="center text-xs">Ліс</th></tr>
            </thead>
            <tbody>
              <tr class="highlight-row"><td>За добу</td><td class="center bold" data-cell="L14">—</td><td class="center bold" data-cell="M14">—</td></tr>
              <tr><td class="bold">площа, га</td><td class="center" data-cell="L15">—</td><td class="center" data-cell="M15">—</td></tr>
              <tr class="highlight-row"><td>З початку року</td><td class="center bold" data-cell="L16">—</td><td class="center bold" data-cell="M16">—</td></tr>
              <tr><td class="bold">площа, га</td><td class="center" data-cell="L17">—</td><td class="center" data-cell="M17">—</td></tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>

    <!-- КОЛОНКА 3 -->
    <div class="grid-column">
      <div class="info-block blue-top">
        <h2>⚡ Електропостачання</h2>
        <div class="table-responsive-wrapper">
          <table class="report-table">
            <thead>
              <tr><th>Причина</th><th class="center text-xs">Повністю</th><th class="center text-xs">Частково</th><th class="center text-xs">Абон.</th></tr>
            </thead>
            <tbody>
              <tr><td class="bold text-orange">Погодні умови</td><td class="center bold" data-cell="L8">—</td><td class="center bold" data-cell="M8">—</td><td class="center bold alert-text" data-cell="N8">—</td></tr>
              <tr><td class="bold text-orange">Бойові дії</td><td class="center bold" data-cell="L9">—</td><td class="center bold" data-cell="M9">—</td><td class="center bold alert-text" data-cell="N9">—</td></tr>
              <tr class="highlight-row"><td class="bold text-orange">Всього</td><td class="center bold" data-cell="L10">—</td><td class="center bold" data-cell="M10">—</td><td class="center bold alert-text" data-cell="N10">—</td></tr>
            </tbody>
          </table>
        </div>
      </div>

      <div class="info-block dark-top">
        <h2>🚀 Наслідки бойових дій</h2>
        <div class="table-responsive-wrapper">
          <table class="report-table">
            <thead>
              <tr><th>Подій</th><th class="center text-xs">Доба</th><th class="center text-xs">2026</th><th class="center text-xs">Всього</th></tr>
            </thead>
            <tbody>
              <tr><td class="bold">Пожежі (бойові дії)</td><td class="center bold" data-cell="G4">—</td><td class="center" data-cell="H4">—</td><td class="center" data-cell="I4">—</td></tr>
              <tr><td class="bold">Пожежі із залученням</td><td class="center bold" data-cell="G5">—</td><td class="center" data-cell="H5">—</td><td class="center" data-cell="I5">—</td></tr>
              <tr class="thick-row border-double"><td class="bold">Обстріли</td><td class="center bold" data-cell="G6">—</td><td class="center" data-cell="H6">—</td><td class="center" data-cell="I6">—</td></tr>
              <tr><td class="indent-cell">пошкоджено будівлі</td><td class="center bold" data-cell="G7">—</td><td class="center" data-cell="H7">—</td><td class="center" data-cell="I7">—</td></tr>
              <tr><td class="indent-cell">пошкоджено техніку</td><td class="center bold" data-cell="G8">—</td><td class="center" data-cell="H8">—</td><td class="center" data-cell="I8">—</td></tr>
              <tr><td class="indent-cell">врятовані</td><td class="center bold" data-cell="G9">—</td><td class="center" data-cell="H9">—</td><td class="center" data-cell="I9">—</td></tr>
              <tr><td class="indent-cell">з них дітей</td><td class="center bold" data-cell="G10">—</td><td class="center" data-cell="H10">—</td><td class="center" data-cell="I10">—</td></tr>
              <tr><td class="indent-cell">загиблі</td><td class="center bold" data-cell="G11">—</td><td class="center" data-cell="H11">—</td><td class="center" data-cell="I11">—</td></tr>
              <tr><td class="indent-cell">з них дітей</td><td class="center bold" data-cell="G12">—</td><td class="center" data-cell="H12">—</td><td class="center" data-cell="I12">—</td></tr>
              <tr><td class="indent-cell">травмовані</td><td class="center bold" data-cell="G13">—</td><td class="center" data-cell="H13">—</td><td class="center" data-cell="I13">—</td></tr>
              <tr><td class="indent-cell">з них дітей</td><td class="center bold" data-cell="G14">—</td><td class="center" data-cell="H14">—</td><td class="center" data-cell="I14">—</td></tr>
              <tr class="highlight-row"><td class="bold">АРР</td><td class="center bold" data-cell="G15">—</td><td class="center" data-cell="H15">—</td><td class="center" data-cell="I15">—</td></tr>
              <tr><td class="bold">Відновлено вікон, шт</td><td class="center bold" data-cell="G16">—</td><td class="center" data-cell="H16">—</td><td class="center" data-cell="I16">—</td></tr>
              <tr><td class="indent-cell">покрівель, м²</td><td class="center bold" data-cell="G17">—</td><td class="center" data-cell="H17">—</td><td class="center" data-cell="I17">—</td></tr>
              <tr class="highlight-row"><td class="bold">Гуманітарна допомога</td><td class="center bold" data-cell="G18">—</td><td class="center" data-cell="H18">—</td><td class="center" data-cell="I18">—</td></tr>
              <tr><td class="indent-cell">вивантажено, т</td><td class="center bold" data-cell="G19">—</td><td class="center" data-cell="H19">—</td><td class="center" data-cell="I19">—</td></tr>
              <tr class="highlight-row"><td class="bold">Евакуація</td><td class="center bold" data-cell="G20">—</td><td class="center" data-cell="H20">—</td><td class="center" data-cell="I20">—</td></tr>
              <tr><td class="indent-cell">евакуйовано осіб</td><td class="center bold" data-cell="G21">—</td><td class="center" data-cell="H21">—</td><td class="center" data-cell="I21">—</td></tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>

  </main>
</div>
</section>

<!-- ===== BURGER BUTTON (видно завжди) ===== -->
<button class="burger-btn" id="burgerBtn" aria-label="Меню" onclick="toggleSidebar()">
  <span></span><span></span><span></span>
</button>

<!-- OVERLAY -->
<div class="sidebar-overlay" id="sidebarOverlay" onclick="toggleSidebar()"></div>

<!-- SIDEBAR -->
<nav class="sidebar" id="sidebar">
  <div class="sidebar-header">
    <h3>📋 Розділи</h3>
  </div>
  <div class="sidebar-nav">
    <a href="#" onclick="showSection('operational'); return false;"><span class="nav-num"></span>🚒 Оперативна інформація</a> 
<a href="#" onclick="toggleAnalyticsMenu(); return false;">
    <span class="nav-num"></span>
    <span class="nav-icon">📊</span>
    Аналітичні дані
    <span id="analyticsArrow" style="margin-left:auto;">▼</span>
</a>

<div id="analyticsSubmenu" style="display:none;">

    <a href="https://firms.modaps.eosdis.nasa.gov/map/#d:24hrs;@33.698,51.886,11.328z"
       target="_blank"
       rel="noopener noreferrer"
       style="padding-left:45px;">
       <span class="nav-icon">🔥</span>
       Термоточки
    </a>

    <a href="https://openinframap.org/#8.99/50.85/34.7987/A,B,I,L,O,P,S,T,W"
       target="_blank"
       rel="noopener noreferrer"
       style="padding-left:45px;">
       <span class="nav-icon">⚡</span>
       Об'єкти енергетики
    </a>

    <a href="https://maps.visicom.ua/c/34.33022,51.14261,14/r/uc0jgxh9g6,uc0jgzb8nh/m/uc0jgxht73?lang=uk"
       target="_blank"
       rel="noopener noreferrer"
       style="padding-left:45px;">
       <span class="nav-icon">🗺️</span>
       Візіком
    </a>

    <a href="https://www.ventusky.com/uk#p=50.76;34.14;7"
       target="_blank"
       rel="noopener noreferrer"
       style="padding-left:45px;">
       <span class="nav-icon">💧</span>
       Техніка по області
    </a>
</div>

<a href="#" onclick="toggleNormativnyMenu(); return false;">
    <span class="nav-num"></span>
    <span class="nav-icon">📁</span>
    Нормативні документи
    <span id="normativnyArrow" style="margin-left:auto;">▼</span>
</a>

<div id="normativnySubmenu" style="display:none;">
    <a href="https://zakon.rada.gov.ua/laws/show/z0534-22#Text"
       target="_blank"
       rel="noopener noreferrer"
       style="padding-left:45px;">
       <span class="nav-icon"></span>
       116
    </a>
    <a href="https://zakon.rada.gov.ua/laws/show/z0534-22#Text"
       target="_blank"
       rel="noopener noreferrer"
       style="padding-left:45px;">
       <span class="nav-icon"></span>
       780
    </a>

    <a href="#" style="padding-left:45px;"><span class="nav-icon">📄</span> Документ 3</a>
    <a href="#" style="padding-left:45px;"><span class="nav-icon">📄</span> Документ 4</a>
    <a href="#" style="padding-left:45px;"><span class="nav-icon">📄</span> Документ 5</a>
    <a href="#" style="padding-left:45px;"><span class="nav-icon">📄</span> Документ 6</a>
    <a href="#" style="padding-left:45px;"><span class="nav-icon">📄</span> Документ 7</a>
    <a href="#" style="padding-left:45px;"><span class="nav-icon">📄</span> Документ 8</a>
    <a href="#" style="padding-left:45px;"><span class="nav-icon">📄</span> Документ 9</a>
    <a href="#" style="padding-left:45px;"><span class="nav-icon">📄</span> Документ 10</a>
</div>

<a href="https://docs.google.com/spreadsheets/d/1U-RaiGh310Y9wzQBOy9fKwtJg5zvz2S4euk2-gdjoh0/edit?gid=0#gid=0"
       target="_blank"
       rel="noopener noreferrer"
       style="padding-left:45px;">
       <span class="nav-icon">⛑️</span>
       Техні по області
    </a>
    <a href="#"><span class="nav-num">07</span><span class="nav-icon">📄</span>Стройова записка</a>

   <a href="https://www.google.com/maps/d/edit?mid=1CmrvY-GGd4IFfd1AoOHC_ccLGsNcjyE&ll=51.317472168470005%2C34.479718761653615&z=8"
       target="_blank"
       rel="noopener noreferrer"
       style="padding-left:45px;">
       <span class="nav-icon">🗺️</span>
       Карта планових цілей
    </a>

    <a href="https://www.google.com/maps/d/edit?mid=1YIGyP-v3Wllimjc-1i5Gq9ntygp1SL0&ll=51.11818004701509%2C34.09933584093874&z=12"
       target="_blank"
       rel="noopener noreferrer"
       style="padding-left:45px;">
       <span class="nav-icon">🗺️</span>
       Карта об'єктів життєзабезпеченя
    </a>


<!-- ===== НАВІГАЦІЯ МІЖ СТОРІНКАМИ ===== -->
<script>
  var mapInitialized = false;

  function showSection(name) {
    document.getElementById('page-home').style.display = 'none';
    document.getElementById('page-operational').classList.remove('active');

    if (name === 'operational') {
      document.getElementById('page-operational').classList.add('active');
      if (!mapInitialized) {
        mapInitialized = true;
        initMap();
        initSync();
      }
    } else {
      document.getElementById('page-home').style.display = 'flex';
    }
    toggleSidebar(true);
  }

  function goHome() {
    document.getElementById('page-operational').classList.remove('active');
    document.getElementById('page-home').style.display = 'flex';
  }

  function toggleSidebar(forceClose) {
    var sidebar = document.getElementById('sidebar');
    var overlay = document.getElementById('sidebarOverlay');
    var burger  = document.getElementById('burgerBtn');
    var isOpen;
    if (forceClose === true) {
      isOpen = false;
      sidebar.classList.remove('open');
    } else {
      isOpen = sidebar.classList.toggle('open');
    }
    overlay.classList.toggle('active', isOpen);
    burger.classList.toggle('open', isOpen);
  }
</script>

<!-- ===== КАРТА (ініціалізується лише при відкритті розділу) ===== -->
<script>
function initMap() {
  var MAP_API_URL = 'https://script.google.com/macros/s/AKfycbyRr506heAW2tNKBju72v-SfGBOizPGt3D-Iok5MURT0JqeAzyPQkQWmGeT6ezl6Wy1Hg/exec';

  var LAYERS = [
    { name: 'Надзвичайні події', color: '#ef4444', icon: '⚠️' },
    { name: 'ВНП',              color: '#3b82f6', icon: '💣' },
    { name: 'Бойові дії',       color: '#eab308', icon: '🚀' },
    { name: 'Пожежі',           color: '#f97316', icon: '🔥' }
  ];

  var map = L.map('open-dsns-map', { zoomControl: true, scrollWheelZoom: true, tap: true })
             .setView([51.5, 34.0], 8);

  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '© <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a>',
    maxZoom: 19
  }).addTo(map);

  // карта мусить перерахувати свій розмір, коли контейнер стає видимим
  setTimeout(function() { map.invalidateSize(); }, 100);

  var layerGroups  = {};
  var layerVisible = {};

  function makeMarker(coords, color, layerName, icon, desc) {
    var size = window.innerWidth < 600 ? 24 : 30;
    var divIcon = L.divIcon({
      html: '<div style="font-size:' + size + 'px; line-height:1; filter: drop-shadow(0 1px 4px rgba(0,0,0,0.8)); cursor:pointer;">' + icon + '</div>',
      className: '',
      iconSize: [size, size],
      iconAnchor: [size / 2, size / 2],
      popupAnchor: [0, -(size / 2 + 4)]
    });
    return L.marker(coords, { icon: divIcon }).bindPopup(
      '<div class="popup-layer" style="color:' + color + '">' + icon + ' ' + layerName + '</div>' +
      '<div class="popup-desc">'   + (desc || '—') + '</div>' +
      '<div class="popup-coords">📍 ' + coords[0].toFixed(5) + ', ' + coords[1].toFixed(5) + '</div>',
      { maxWidth: 240 }
    );
  }

  function parseCoords(raw) {
    if (!raw) return null;
    var s = String(raw).trim().replace(/\s*[;,]\s*/g, ',');
    var p = s.split(',').map(Number).filter(function(n) { return !isNaN(n) && n !== 0; });
    if (p.length < 2) return null;
    var lat = p[0], lng = p[1];
    if (lat < 43 || lat > 54 || lng < 21 || lng > 42) return null;
    return [lat, lng];
  }

  function loadLayer(layer, callback) {
    var group = L.layerGroup().addTo(map);
    layerGroups[layer.name]  = group;
    layerVisible[layer.name] = true;
    var count = 0;

    var id     = '_cb_' + Date.now() + '_' + Math.floor(Math.random() * 999999);
    var script = document.createElement('script');
    var timer  = setTimeout(function() { finish(); }, 15000);

    function finish() {
      clearTimeout(timer);
      try { delete window[id]; } catch(e) {}
      if (script.parentNode) script.parentNode.removeChild(script);
      callback({ name: layer.name, color: layer.color, icon: layer.icon, count: count });
    }

    window[id] = function(rows) {
      if (Array.isArray(rows)) {
        rows.forEach(function(row) {
          var coords = parseCoords(row.coords);
          if (!coords) return;
          count++;
          makeMarker(coords, layer.color, layer.name, layer.icon, row.desc).addTo(group);
        });
      }
      finish();
    };

    script.src = MAP_API_URL + '?sheet=' + encodeURIComponent(layer.name) + '&callback=' + id;
    script.onerror = function() { finish(); };
    document.head.appendChild(script);
  }

  function buildLegend(results) {
    var container = document.getElementById('map-legend-items');
    results.forEach(function(r) {
      var div = document.createElement('div');
      div.className = 'legend-item';
      div.innerHTML =
        '<span style="font-size:16px; line-height:1;">' + r.icon + '</span>' +
        '<span style="color:#e2e8f0">' + r.name +
        ' <span style="color:#64748b">(' + r.count + ')</span></span>';
      div.addEventListener('click', function() {
        if (layerVisible[r.name]) {
          map.removeLayer(layerGroups[r.name]);
          layerVisible[r.name] = false;
          div.classList.add('hidden-layer');
        } else {
          layerGroups[r.name].addTo(map);
          layerVisible[r.name] = true;
          div.classList.remove('hidden-layer');
        }
      });
      container.appendChild(div);
    });
    document.getElementById('map-legend').style.display = 'block';
  }

  var results = [];
  var done    = 0;

  LAYERS.forEach(function(layer) {
    loadLayer(layer, function(result) {
      results.push(result);
      done++;
      if (done < LAYERS.length) return;

      var total = results.reduce(function(s, r) { return s + r.count; }, 0);
      var dot   = document.getElementById('map-status-dot');
      var text  = document.getElementById('map-status-text');

      dot.classList.remove('loading');
      if (total > 0) {
        dot.classList.add('ok');
        text.textContent = total + ' подій · щойно';
      } else {
        text.style.color = '#ef4444';
        text.textContent = 'Даних немає';
      }

      buildLegend(results);

      var pts = [];
      Object.values(layerGroups).forEach(function(g) {
        g.eachLayer(function(l) { if (l.getLatLng) pts.push(l.getLatLng()); });
      });
      if (pts.length) {
        var fg = L.featureGroup(pts.map(function(p) { return L.circleMarker(p); }));
        map.fitBounds(fg.getBounds().pad(0.15));
      }
    });
  });
}
</script>

<!-- ===== СИНХРОНІЗАЦІЯ ТАБЛИЦІ ===== -->
<script>
function initSync() {
  var API_URL  = 'https://script.google.com/macros/s/AKfycby2jNEZR3OV_R1r4v7TWS2dK7qaevHzAmZJAqRoKktrD0mr6SGLBdfOVJySRBZ7azJL2g/exec';
  var INTERVAL = 5 * 60 * 1000;

  function setStatus(state, text) {
    var el = document.getElementById('sync-status');
    if (!el) return;
    el.textContent = text;
    el.className = 'sync-' + state;
  }

  function cellToIndex(ref) {
    var match = ref.match(/^([A-Z]+)(\d+)$/i);
    if (!match) return null;
    var col = match[1].toUpperCase().split('').reduce(function(acc, ch) {
      return acc * 26 + ch.charCodeAt(0) - 64;
    }, 0) - 1;
    var row = parseInt(match[2]) - 1;
    return { row: row, col: col };
  }

  function syncSheet() {
    setStatus('loading', '🔄');
    fetch(API_URL, { redirect: 'follow' })
      .then(function(res) { if (!res.ok) throw new Error('HTTP ' + res.status); return res.json(); })
      .then(function(data) {
        document.querySelectorAll('[data-cell]').forEach(function(td) {
          var idx = cellToIndex(td.dataset.cell);
          if (!idx) return;
          var val = data[idx.row] && data[idx.row][idx.col];
          if (val !== undefined && val !== '') td.textContent = val;
        });
        var t = new Date().toLocaleTimeString('uk-UA', { hour: '2-digit', minute: '2-digit' });
        setStatus('ok', '✅ ' + t);
      })
      .catch(function(err) { setStatus('error', '❌'); });
  }

  syncSheet();
  setInterval(syncSheet, INTERVAL);
}
</script>

<!-- ===== ГОДИННИК + АКОРДЕОН ===== -->
<script>
function updateClock() {
  var now = new Date();
  var t = now.toLocaleTimeString('uk-UA', { hour: '2-digit', minute: '2-digit', second: '2-digit' });
  var d = now.toLocaleDateString('uk-UA', { day: '2-digit', month: '2-digit', year: 'numeric' });
  var el = document.getElementById('dashboardClock');
  if (el) el.textContent = t + ' ' + d;
}
setInterval(updateClock, 1000);
updateClock();

function toggleAccordion(btn) {
  btn.classList.toggle('open');
  var body = btn.nextElementSibling;
  body.classList.toggle('open');
}
</script>
<script>
function toggleAnalyticsMenu() {
    const menu = document.getElementById('analyticsSubmenu');
    const arrow = document.getElementById('analyticsArrow');

    if (menu.style.display === 'none' || menu.style.display === '') {
        menu.style.display = 'block';
        arrow.textContent = '▲';
    } else {
        menu.style.display = 'none';
        arrow.textContent = '▼';
    }
}

function toggleNormativnyMenu() {
    const menu = document.getElementById('normativnySubmenu');
    const arrow = document.getElementById('normativnyArrow');

    if (menu.style.display === 'none' || menu.style.display === '') {
        menu.style.display = 'block';
        arrow.textContent = '▲';
    } else {
        menu.style.display = 'none';
        arrow.textContent = '▼';
    }
}
</script>


<script>
async function saveOperationalPDF() {
  const element = document.querySelector('.dashboard-wrapper');

  const canvas = await html2canvas(element, {
      scale: 2,
      useCORS: true,
      backgroundColor: '#0f172a'
  });

  const imgData = canvas.toDataURL('image/jpeg', 1.0);

  const { jsPDF } = window.jspdf;

  const pdf = new jsPDF({
      orientation: 'landscape',
      unit: 'mm',
      format: 'a4'
  });

  const pageWidth = 297;
  const pageHeight = 210;
  const margin = 5;

  const usableWidth = pageWidth - margin * 2;
  const imgWidth = usableWidth;
  const imgHeight = (canvas.height * imgWidth) / canvas.width;

  let heightLeft = imgHeight;
  let position = margin;

  pdf.addImage(imgData, 'JPEG', margin, position, imgWidth, imgHeight);

  heightLeft -= (pageHeight - margin * 2);

  while (heightLeft > 0) {
      position = heightLeft - imgHeight + margin;
      pdf.addPage();
      pdf.addImage(imgData, 'JPEG', margin, position, imgWidth, imgHeight);
      heightLeft -= (pageHeight - margin * 2);
  }

  const now = new Date();
  const fileName =
      'Оперативна_інформація_' +
      now.toLocaleDateString('uk-UA').replace(/\./g,'-') +
      '.pdf';

  pdf.save(fileName);
}
</script>


</body>
</html>
