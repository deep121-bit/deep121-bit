<svg width="1280" height="720" viewBox="0 0 1280 720" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0D1117"/>
      <stop offset="55%" stop-color="#111827"/>
      <stop offset="100%" stop-color="#0D1117"/>
    </linearGradient>
    <linearGradient id="nameGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#FF4D8D"/>
      <stop offset="50%" stop-color="#7C3AED"/>
      <stop offset="100%" stop-color="#00E5FF"/>
    </linearGradient>
    <clipPath id="roundedBanner"><rect width="1280" height="720" rx="28"/></clipPath>
  </defs>

  <g clip-path="url(#roundedBanner)">
    <!-- Background -->
    <rect width="1280" height="720" fill="url(#bgGrad)"/>

    <!-- Greeting -->
    <text x="45" y="105" font-family="Consolas, monospace" font-size="30" fill="#B0BEC5">Hi 👋, I'm</text>

    <!-- Name -->
    <text x="45" y="175" font-family="'Brush Script MT', cursive" font-size="64" font-weight="bold" fill="url(#nameGrad)">
      Deepak Maurya
    </text>

    <!-- Role -->
    <text x="45" y="225" font-family="Consolas, monospace" font-size="26" fill="#00E5FF">&gt; Data Analyst / AI Engineer</text>

    <!-- Tagline -->
    <rect x="45" y="255" width="620" height="55" rx="10" fill="#ffffff08" stroke="#7C3AED44"/>
    <text x="60" y="290" font-family="Consolas, monospace" font-size="18" fill="#B0BEC5">
      "Building Intelligent Systems with Data &amp; AI"
    </text>

    <!-- Buttons -->
    <g font-family="Consolas, monospace" font-size="16" font-weight="bold">
      <g>
        <rect x="45" y="400" width="150" height="44" rx="10" fill="#7C3AED"/>
        <text x="120" y="427" text-anchor="middle" fill="#FFFFFF">GitHub</text>
      </g>
      <g>
        <rect x="205" y="400" width="150" height="44" rx="10" fill="none" stroke="#00E5FF" stroke-width="2"/>
        <text x="280" y="427" text-anchor="middle" fill="#00E5FF">LinkedIn</text>
      </g>
      <g>
        <rect x="365" y="400" width="150" height="44" rx="10" fill="none" stroke="#FF4D8D" stroke-width="2"/>
        <text x="440" y="427" text-anchor="middle" fill="#FF4D8D">Email</text>
      </g>
    </g>

    <!-- Location/Education -->
    <g font-family="Consolas, monospace" font-size="15" fill="#B0BEC5">
      <text x="45" y="500">📍 Delhi, India</text>
      <text x="230" y="500">🎓 MCA @ Chandigarh University</text>
      <text x="560" y="500">💼 Open to Data Analyst / AI Engineer roles</text>
    </g>

    <!-- Water image at bottom -->
    <image href="assets/images/water.png" 
           x="0" y="550" 
           width="1280" height="170" 
           preserveAspectRatio="xMidYMid slice" 
           opacity="0.7">
      <!-- Wave animation -->
      <animateTransform attributeName="transform" 
                        type="translate" 
                        values="0,0; 0,10; 0,0" 
                        dur="4s" 
                        repeatCount="indefinite"/>
    </image>
  </g>

  <!-- Border -->
  <rect x="1" y="1" width="1278" height="718" rx="28" fill="none" stroke="#7C3AED55" stroke-width="2"/>
</svg>
