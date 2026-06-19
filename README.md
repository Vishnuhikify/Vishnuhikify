<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 320" width="1200" height="320" font-family="'Segoe UI', Arial, sans-serif">
  <defs>
    <radialGradient id="atmos" cx="25%" cy="20%" r="95%">
      <stop offset="0%" stop-color="#1a2347"/>
      <stop offset="55%" stop-color="#0f1530"/>
      <stop offset="100%" stop-color="#080b1a"/>
    </radialGradient>
    <radialGradient id="gPurple" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#7c5cff" stop-opacity="0.55"/><stop offset="100%" stop-color="#7c5cff" stop-opacity="0"/>
    </radialGradient>
    <radialGradient id="gCyan" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#22d3ee" stop-opacity="0.45"/><stop offset="100%" stop-color="#22d3ee" stop-opacity="0"/>
    </radialGradient>
    <radialGradient id="gPink" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#ec4899" stop-opacity="0.4"/><stop offset="100%" stop-color="#ec4899" stop-opacity="0"/>
    </radialGradient>
    <linearGradient id="nameGrad" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#22d3ee"/><stop offset="50%" stop-color="#7c5cff"/><stop offset="100%" stop-color="#ec4899"/>
    </linearGradient>
    <linearGradient id="cubeT" x1="0" y1="0" x2="1" y2="1"><stop offset="0%" stop-color="#8b6dff"/><stop offset="100%" stop-color="#6d4fe0"/></linearGradient>
    <linearGradient id="cubeL" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#5a3fc0"/><stop offset="100%" stop-color="#3d2a8c"/></linearGradient>
    <linearGradient id="cubeR" x1="0" y1="0" x2="0" y2="1"><stop offset="0%" stop-color="#4a32a8" stop-color-opacity="1"/><stop offset="100%" stop-color="#2e1f6e"/></linearGradient>
    <style>
      @keyframes spin   { 0%{transform:rotate(0)} 100%{transform:rotate(360deg)} }
      @keyframes floaty { 0%,100%{transform:translateY(0)} 50%{transform:translateY(-14px)} }
      @keyframes floaty2{ 0%,100%{transform:translateY(0)} 50%{transform:translateY(-9px)} }
      @keyframes pulse  { 0%,100%{opacity:.5} 50%{opacity:1} }
      @keyframes drift  { 0%{transform:translate(0,0)} 100%{transform:translate(30px,18px)} }
      @keyframes fadeUp { 0%{opacity:0;transform:translateY(16px)} 100%{opacity:1;transform:none} }
      @keyframes dash   { to { stroke-dashoffset: -380; } }
      .cube  { transform-box:fill-box; transform-origin:center; animation: floaty 6s ease-in-out infinite; }
      .ring  { transform-box:fill-box; transform-origin:center; animation: spin 18s linear infinite; }
      .ring2 { transform-box:fill-box; transform-origin:center; animation: spin 26s linear infinite reverse; }
      .orb1  { transform-box:fill-box; transform-origin:center; animation: floaty2 5.5s ease-in-out infinite .3s; }
      .orb2  { transform-box:fill-box; transform-origin:center; animation: floaty2 6.4s ease-in-out infinite .8s; }
      .g1{animation:pulse 7s ease-in-out infinite} .g2{animation:pulse 9s ease-in-out infinite 1s} .g3{animation:pulse 8s ease-in-out infinite .5s}
      .drift{animation:drift 20s ease-in-out infinite alternate}
      .t1{opacity:0;animation:fadeUp .8s ease-out .2s forwards}
      .t2{opacity:0;animation:fadeUp .8s ease-out .5s forwards}
      .t3{opacity:0;animation:fadeUp .8s ease-out .8s forwards}
      .flow{stroke-dasharray:6 10;animation:dash 5s linear infinite}
    </style>
  </defs>

  <rect width="1200" height="320" rx="20" fill="url(#atmos)"/>
  <circle class="g1 drift" cx="200" cy="120" r="240" fill="url(#gPurple)"/>
  <circle class="g2 drift" cx="1020" cy="250" r="250" fill="url(#gCyan)"/>
  <circle class="g3 drift" cx="640" cy="60"  r="200" fill="url(#gPink)"/>

  <!-- subtle circuit lines -->
  <g stroke="#7c5cff" stroke-opacity="0.18" fill="none" stroke-width="1.5">
    <path class="flow" d="M0,260 H120 V210 H210"/>
    <path class="flow" d="M0,80 H80 V130 H180"/>
    <path class="flow" d="M1200,90 H1080 V150 H1000"/>
  </g>

  <!-- ===== left text ===== -->
  <text class="t1" x="64" y="108" font-size="22" fill="#8b95b8" letter-spacing="6">FULL-STACK  DEVELOPER</text>
  <text class="t2" x="60" y="186" font-size="74" font-weight="800" fill="url(#nameGrad)" letter-spacing="-1">Vishnu Prasad</text>
  <text class="t3" x="64" y="228" font-size="21" fill="#aeb6d6">IoT  ·  Machine Learning  ·  Cybersecurity  ·  Cloud</text>
  <g class="t3" font-family="Arial" font-size="14" fill="#aeb6d6">
    <rect x="64"  y="252" width="132" height="32" rx="16" fill="#ffffff" fill-opacity="0.06" stroke="#7c5cff" stroke-opacity="0.3"/>
    <text x="84"  y="273">🤖 AI &amp; ML</text>
    <rect x="208" y="252" width="116" height="32" rx="16" fill="#ffffff" fill-opacity="0.06" stroke="#22d3ee" stroke-opacity="0.3"/>
    <text x="228" y="273">📡 IoT</text>
    <rect x="336" y="252" width="160" height="32" rx="16" fill="#ffffff" fill-opacity="0.06" stroke="#ec4899" stroke-opacity="0.3"/>
    <text x="356" y="273">🔐 Cybersecurity</text>
  </g>

  <!-- ===== right: 3D isometric cube + orbiting rings ===== -->
  <g transform="translate(980,160)">
    <!-- orbit rings -->
    <ellipse class="ring"  cx="0" cy="0" rx="150" ry="56" fill="none" stroke="#7c5cff" stroke-opacity="0.35" stroke-width="2"/>
    <ellipse class="ring2" cx="0" cy="0" rx="120" ry="120" fill="none" stroke="#22d3ee" stroke-opacity="0.25" stroke-width="2" stroke-dasharray="4 10"/>
    <!-- orbiting orbs -->
    <circle class="orb1" cx="150" cy="0" r="7" fill="#22d3ee"/>
    <circle class="orb2" cx="-120" cy="40" r="6" fill="#ec4899"/>
    <circle class="orb1" cx="0" cy="-120" r="6" fill="#7c5cff"/>

    <!-- isometric 3D cube -->
    <g class="cube">
      <!-- top face -->
      <polygon points="0,-70 70,-32 0,6 -70,-32" fill="url(#cubeT)" stroke="#b9a6ff" stroke-opacity="0.5"/>
      <!-- left face -->
      <polygon points="-70,-32 0,6 0,86 -70,48" fill="url(#cubeL)" stroke="#b9a6ff" stroke-opacity="0.3"/>
      <!-- right face -->
      <polygon points="70,-32 0,6 0,86 70,48" fill="url(#cubeR)" stroke="#b9a6ff" stroke-opacity="0.3"/>
      <!-- code glyphs on faces -->
      <text x="-44" y="18" font-size="22" font-family="monospace" fill="#d9ccff" fill-opacity="0.85">&lt;/&gt;</text>
      <text x="20" y="52" font-size="20" font-family="monospace" fill="#c7b6ff" fill-opacity="0.7">{ }</text>
      <text x="-12" y="-30" font-size="18" font-family="monospace" fill="#ffffff" fill-opacity="0.55">V</text>
    </g>
  </g>
</svg>
