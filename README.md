<svg xmlns="http://www.w3.org/2000/svg" width="1280" height="120" viewBox="0 0 1280 120" preserveAspectRatio="xMidYMid meet">
  <defs>
    <!-- grid cell pattern: square cell with inner dark square -->
    <pattern id="cell" width="16" height="16" patternUnits="userSpaceOnUse">
      <rect width="16" height="16" fill="transparent"/>
      <rect x="2" y="2" width="12" height="12" rx="2" fill="#0b1115"/>
    </pattern>
  </defs>

  <!-- background -->
  <rect width="1280" height="120" rx="6" fill="#05060a"/>

  <!-- grid area -->
  <g transform="translate(24,16)">
    <rect width="1232" height="64" rx="4" fill="url(#cell)"/>
    <!-- optional subtle overlay to darken the gaps -->
    <rect width="1232" height="64" rx="4" fill="rgba(0,0,0,0.12)"/>
  </g>

  <!-- colored pixel clusters (positions are multiples of 16 from the grid origin at x=24,y=16) -->
  <g transform="translate(24,16)">
    <!-- left accent -->
    <rect x="{x1}" y="{y1}" width="12" height="12" rx="2" fill="#0ea5a4" />
  </g>

  <!-- Real clusters placed by explicit coordinates so they align with grid -->

  <!-- Right-side green cluster -->
  <g transform="translate(24,16)">
    <rect x="680" y="8" width="12" height="12" rx="2" fill="#064e3b"/>
    <rect x="696" y="8" width="12" height="12" rx="2" fill="#0ea5a4"/>
    <rect x="712" y="8" width="12" height="12" rx="2" fill="#0ea5a4"/>

    <rect x="680" y="24" width="12" height="12" rx="2" fill="#063b2d"/>
    <rect x="712" y="40" width="12" height="12" rx="2" fill="#0ea5a4"/>
  </g>

  <!-- Small magenta cluster near the green cluster -->
  <g transform="translate(24,16)">
    <rect x="744" y="24" width="12" height="12" rx="2" fill="#a21caf"/>
    <rect x="760" y="24" width="12" height="12" rx="2" fill="#7c0570"/>
    <rect x="744" y="40" width="12" height="12" rx="2" fill="#a21caf"/>
  </g>

  <!-- scattered accents to match the sample -->
  <g transform="translate(24,16)">
    <rect x="720" y="0" width="12" height="12" rx="2" fill="#0ea5a4"/>
    <rect x="736" y="16" width="12" height="12" rx="2" fill="#0ea5a4"/>
    <rect x="688" y="56" width="12" height="12" rx="2" fill="#063b2d"/>
    <rect x="96" y="8" width="12" height="12" rx="2" fill="#0ea5a4"/>
  </g>

  <!-- thin progress bar below the grid -->
  <rect x="24" y="96" width="540" height="8" rx="4" fill="#063b2d" opacity="0.98"/>

  <!-- subtle glow behind the clusters -->
  <g opacity="0.10" transform="translate(24,16)">
    <ellipse cx="760" cy="26" rx="46" ry="18" fill="#0ea5a4"/>
  </g>
</svg>
