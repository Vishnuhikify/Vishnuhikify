<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 760 130" width="760" height="130" font-family="'Segoe UI', Verdana, Arial, sans-serif">
  <defs>
    <linearGradient id="hiGrad" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#22d3ee"/><stop offset="50%" stop-color="#7c5cff"/><stop offset="100%" stop-color="#ec4899"/>
      <animateTransform attributeName="gradientTransform" type="translate" values="-0.25 0; 0.25 0; -0.25 0" dur="7s" repeatCount="indefinite"/>
    </linearGradient>
    <!-- 3D extrude: stacked dark copies behind the main text -->
    <filter id="depth" x="-10%" y="-20%" width="120%" height="160%">
      <feDropShadow dx="2" dy="2" stdDeviation="0" flood-color="#3d2a8c" flood-opacity="0.9"/>
      <feDropShadow dx="4" dy="4" stdDeviation="0" flood-color="#2e1f6e" flood-opacity="0.8"/>
      <feDropShadow dx="6" dy="6" stdDeviation="0" flood-color="#1e1450" flood-opacity="0.7"/>
      <feDropShadow dx="9" dy="9" stdDeviation="3" flood-color="#000000" flood-opacity="0.45"/>
    </filter>
  </defs>

  <!-- waving hand (rotates back and forth via SMIL) -->
  <text x="36" y="86" font-size="62">
    👋
    <animateTransform attributeName="transform" type="rotate" values="0 50 70; 18 50 70; -8 50 70; 14 50 70; 0 50 70" dur="2.2s" repeatCount="indefinite"/>
  </text>

  <!-- 3D extruded title -->
  <text x="120" y="84" font-size="58" font-weight="800" fill="url(#hiGrad)" filter="url(#depth)" letter-spacing="-1">
    Hi there, I'm Vishnu
    <animateTransform attributeName="transform" type="translate" values="0 0; 0 -5; 0 0" dur="4s" repeatCount="indefinite"/>
  </text>
</svg>
