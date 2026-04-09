<svg xmlns="http://www.w3.org/2000/svg" width="800" height="400" viewBox="0 0 800 400" style="background-color: #000000;">
  <defs>
    <style>
      /* Even columns (2,4,6,8...) - Move DOWN */
      @keyframes fallDown {
        0% { transform: translateY(-100px); opacity: 0; }
        10% { opacity: 1; }
        90% { opacity: 0.8; }
        100% { transform: translateY(300px); opacity: 0; }
      }
      
      /* Odd columns (1,3,5,7...) - Move UP */
      @keyframes riseUp {
        0% { transform: translateY(300px); opacity: 0; }
        10% { opacity: 1; }
        90% { opacity: 0.8; }
        100% { transform: translateY(-100px); opacity: 0; }
      }
      
      /* Column classes */
      .col1, .col3, .col5, .col7, .col9, .col11, .col13, .col15 { animation: riseUp 5s infinite linear; }
      .col2, .col4, .col6, .col8, .col10, .col12, .col14, .col16 { animation: fallDown 5s infinite linear; }
      
      /* Delay each column for wave effect */
      .col1 { animation-delay: 0s; }
      .col2 { animation-delay: 0.3s; }
      .col3 { animation-delay: 0.6s; }
      .col4 { animation-delay: 0.9s; }
      .col5 { animation-delay: 1.2s; }
      .col6 { animation-delay: 1.5s; }
      .col7 { animation-delay: 1.8s; }
      .col8 { animation-delay: 2.1s; }
      .col9 { animation-delay: 2.4s; }
      .col10 { animation-delay: 2.7s; }
      .col11 { animation-delay: 3.0s; }
      .col12 { animation-delay: 3.3s; }
      .col13 { animation-delay: 3.6s; }
      .col14 { animation-delay: 3.9s; }
      .col15 { animation-delay: 4.2s; }
      .col16 { animation-delay: 4.5s; }
      
      .binary {
        font-family: 'Courier New', monospace;
        font-size: 16px;
        fill: #00ff00;
      }
      
      .dim {
        opacity: 0.3;
      }
      
      .bright {
        opacity: 1;
        fill: #ffffff;
      }
      
      /* Glow effect for some digits */
      @keyframes glow {
        0%, 100% { opacity: 0.8; }
        50% { opacity: 1; fill: #ffffff; }
      }
      
      .glow {
        animation: glow 2s infinite;
      }
    </style>
  </defs>
  
  <!-- Background -->
  <rect width="800" height="400" fill="#000000"/>
  
  <!-- COLUMN 1 (ODD - moves UP) -->
  <g class="col1">
    <text class="binary" x="30" y="20">1</text>
    <text class="binary dim" x="30" y="45">0</text>
    <text class="binary" x="30" y="70">1</text>
    <text class="binary dim" x="30" y="95">1</text>
    <text class="binary glow" x="30" y="120">0</text>
    <text class="binary dim" x="30" y="145">1</text>
    <text class="binary" x="30" y="170">0</text>
    <text class="binary dim" x="30" y="195">1</text>
    <text class="binary" x="30" y="220">1</text>
    <text class="binary dim" x="30" y="245">0</text>
    <text class="binary" x="30" y="270">1</text>
    <text class="binary dim" x="30" y="295">0</text>
    <text class="binary glow" x="30" y="320">0</text>
    <text class="binary dim" x="30" y="345">1</text>
    <text class="binary" x="30" y="370">1</text>
  </g>
  
  <!-- COLUMN 2 (EVEN - moves DOWN) -->
  <g class="col2">
    <text class="binary" x="70" y="20">0</text>
    <text class="binary dim" x="70" y="45">1</text>
    <text class="binary" x="70" y="70">0</text>
    <text class="binary dim" x="70" y="95">1</text>
    <text class="binary" x="70" y="120">1</text>
    <text class="binary dim" x="70" y="145">0</text>
    <text class="binary glow" x="70" y="170">1</text>
    <text class="binary dim" x="70" y="195">0</text>
    <text class="binary" x="70" y="220">0</text>
    <text class="binary dim" x="70" y="245">1</text>
    <text class="binary" x="70" y="270">0</text>
    <text class="binary dim" x="70" y="295">1</text>
    <text class="binary" x="70" y="320">1</text>
    <text class="binary dim glow" x="70" y="345">0</text>
    <text class="binary" x="70" y="370">0</text>
  </g>
  
  <!-- COLUMN 3 (ODD - moves UP) -->
  <g class="col3">
    <text class="binary" x="110" y="20">1</text>
    <text class="binary dim" x="110" y="45">1</text>
    <text class="binary glow" x="110" y="70">0</text>
    <text class="binary dim" x="110" y="95">0</text>
    <text class="binary" x="110" y="120">1</text>
    <text class="binary dim" x="110" y="145">1</text>
    <text class="binary" x="110" y="170">0</text>
    <text class="binary dim" x="110" y="195">1</text>
    <text class="binary" x="110" y="220">0</text>
    <text class="binary dim" x="110" y="245">0</text>
    <text class="binary glow" x="110" y="270">1</text>
    <text class="binary dim" x="110" y="295">1</text>
    <text class="binary" x="110" y="320">0</text>
    <text class="binary dim" x="110" y="345">1</text>
    <text class="binary" x="110" y="370">0</text>
  </g>
  
  <!-- COLUMN 4 (EVEN - moves DOWN) -->
  <g class="col4">
    <text class="binary" x="150" y="20">0</text>
    <text class="binary dim" x="150" y="45">0</text>
    <text class="binary" x="150" y="70">1</text>
    <text class="binary dim" x="150" y="95">1</text>
    <text class="binary glow" x="150" y="120">0</text>
    <text class="binary dim" x="150" y="145">0</text>
    <text class="binary" x="150" y="170">1</text>
    <text class="binary dim" x="150" y="195">0</text>
    <text class="binary" x="150" y="220">1</text>
    <text class="binary dim" x="150" y="245">1</text>
    <text class="binary" x="150" y="270">0</text>
    <text class="binary dim glow" x="150" y="295">1</text>
    <text class="binary" x="150" y="320">0</text>
    <text class="binary dim" x="150" y="345">0</text>
    <text class="binary" x="150" y="370">1</text>
  </g>
  
  <!-- COLUMN 5 (ODD - moves UP) -->
  <g class="col5">
    <text class="binary glow" x="190" y="20">1</text>
    <text class="binary dim" x="190" y="45">0</text>
    <text class="binary" x="190" y="70">1</text>
    <text class="binary dim" x="190" y="95">0</text>
    <text class="binary" x="190" y="120">0</text>
    <text class="binary dim" x="190" y="145">1</text>
    <text class="binary" x="190" y="170">1</text>
    <text class="binary dim" x="190" y="195">0</text>
    <text class="binary glow" x="190" y="220">1</text>
    <text class="binary dim" x="190" y="245">0</text>
    <text class="binary" x="190" y="270">0</text>
    <text class="binary dim" x="190" y="295">1</text>
    <text class="binary" x="190" y="320">1</text>
    <text class="binary dim" x="190" y="345">0</text>
    <text class="binary" x="190" y="370">1</text>
  </g>
  
  <!-- COLUMN 6 (EVEN - moves DOWN) -->
  <g class="col6">
    <text class="binary" x="230" y="20">0</text>
    <text class="binary dim glow" x="230" y="45">1</text>
    <text class="binary" x="230" y="70">1</text>
    <text class="binary dim" x="230" y="95">0</text>
    <text class="binary" x="230" y="120">1</text>
    <text class="binary dim" x="230" y="145">0</text>
    <text class="binary" x="230" y="170">0</text>
    <text class="binary dim" x="230" y="195">1</text>
    <text class="binary" x="230" y="220">1</text>
    <text class="binary dim" x="230" y="245">0</text>
    <text class="binary glow" x="230" y="270">1</text>
    <text class="binary dim" x="230" y="295">0</text>
    <text class="binary" x="230" y="320">0</text>
    <text class="binary dim" x="230" y="345">1</text>
    <text class="binary" x="230" y="370">1</text>
  </g>
  
  <!-- COLUMN 7 (ODD - moves UP) -->
  <g class="col7">
    <text class="binary" x="270" y="20">1</text>
    <text class="binary dim" x="270" y="45">1</text>
    <text class="binary" x="270" y="70">0</text>
    <text class="binary dim" x="270" y="95">1</text>
    <text class="binary" x="270" y="120">1</text>
    <text class="binary dim" x="270" y="145">0</text>
    <text class="binary glow" x="270" y="170">0</text>
    <text class="binary dim" x="270" y="195">1</text>
    <text class="binary" x="270" y="220">0</text>
    <text class="binary dim" x="270" y="245">1</text>
    <text class="binary" x="270" y="270">1</text>
    <text class="binary dim" x="270" y="295">0</text>
    <text class="binary" x="270" y="320">1</text>
    <text class="binary dim" x="270" y="345">0</text>
    <text class="binary glow" x="270" y="370">0</text>
  </g>
  
  <!-- COLUMN 8 (EVEN - moves DOWN) -->
  <g class="col8">
    <text class="binary" x="310" y="20">0</text>
    <text class="binary dim" x="310" y="45">1</text>
    <text class="binary glow" x="310" y="70">0</text>
    <text class="binary dim" x="310" y="95">0</text>
    <text class="binary" x="310" y="120">1</text>
    <text class="binary dim" x="310" y="145">1</text>
    <text class="binary" x="310" y="170">0</text>
    <text class="binary dim" x="310" y="195">1</text>
    <text class="binary" x="310" y="220">0</text>
    <text class="binary dim" x="310" y="245">0</text>
    <text class="binary" x="310" y="270">1</text>
    <text class="binary dim" x="310" y="295">1</text>
    <text class="binary" x="310" y="320">0</text>
    <text class="binary dim glow" x="310" y="345">1</text>
    <text class="binary" x="310" y="370">0</text>
  </g>
  
  <!-- COLUMN 9 (ODD - moves UP) -->
  <g class="col9">
    <text class="binary" x="350" y="20">1</text>
    <text class="binary dim" x="350" y="45">0</text>
    <text class="binary" x="350" y="70">0</text>
    <text class="binary dim" x="350" y="95">1</text>
    <text class="binary" x="350" y="120">0</text>
    <text class="binary dim glow" x="350" y="145">1</text>
    <text class="binary" x="350" y="170">1</text>
    <text class="binary dim" x="350" y="195">0</text>
    <text class="binary" x="350" y="220">1</text>
    <text class="binary dim" x="350" y="245">1</text>
    <text class="binary" x="350" y="270">0</text>
    <text class="binary dim" x="350" y="295">0</text>
    <text class="binary glow" x="350" y="320">1</text>
    <text class="binary dim" x="350" y="345">0</text>
    <text class="binary" x="350" y="370">1</text>
  </g>
  
  <!-- COLUMN 10 (EVEN - moves DOWN) -->
  <g class="col10">
    <text class="binary" x="390" y="20">0</text>
    <text class="binary dim" x="390" y="45">1</text>
    <text class="binary" x="390" y="70">1</text>
    <text class="binary dim" x="390" y="95">0</text>
    <text class="binary" x="390" y="120">1</text>
    <text class="binary dim" x="390" y="145">0</text>
    <text class="binary" x="390" y="170">0</text>
    <text class="binary dim" x="390" y="195">1</text>
    <text class="binary glow" x="390" y="220">0</text>
    <text class="binary dim" x="390" y="245">1</text>
    <text class="binary" x="390" y="270">1</text>
    <text class="binary dim" x="390" y="295">0</text>
    <text class="binary" x="390" y="320">1</text>
    <text class="binary dim" x="390" y="345">0</text>
    <text class="binary" x="390" y="370">0</text>
  </g>
  
  <!-- COLUMN 11 (ODD - moves UP) -->
  <g class="col11">
    <text class="binary glow" x="430" y="20">1</text>
    <text class="binary dim" x="430" y="45">1</text>
    <text class="binary" x="430" y="70">0</text>
    <text class="binary dim" x="430" y="95">1</text>
    <text class="binary" x="430" y="120">0</text>
    <text class="binary dim" x="430" y="145">0</text>
    <text class="binary" x="430" y="170">1</text>
    <text class="binary dim" x="430" y="195">1</text>
    <text class="binary" x="430" y="220">0</text>
    <text class="binary dim" x="430" y="245">1</text>
    <text class="binary" x="430" y="270">0</text>
    <text class="binary dim glow" x="430" y="295">1</text>
    <text class="binary" x="430" y="320">1</text>
    <text class="binary dim" x="430" y="345">0</text>
    <text class="binary" x="430" y="370">1</text>
  </g>
  
  <!-- COLUMN 12 (EVEN - moves DOWN) -->
  <g class="col12">
    <text class="binary" x="470" y="20">0</text>
    <text class="binary dim" x="470" y="45">0</text>
    <text class="binary" x="470" y="70">1</text>
    <text class="binary dim" x="470" y="95">0</text>
    <text class="binary glow" x="470" y="120">1</text>
    <text class="binary dim" x="470" y="145">1</text>
    <text class="binary" x="470" y="170">0</text>
    <text class="binary dim" x="470" y="195">0</text>
    <text class="binary" x="470" y="220">1</text>
    <text class="binary dim" x="470" y="245">0</text>
    <text class="binary" x="470" y="270">1</text>
    <text class="binary dim" x="470" y="295">1</text>
    <text class="binary" x="470" y="320">0</text>
    <text class="binary dim" x="470" y="345">1</text>
    <text class="binary" x="470" y="370">0</text>
  </g>
  
  <!-- COLUMN 13 (ODD - moves UP) -->
  <g class="col13">
    <text class="binary" x="510" y="20">1</text>
    <text class="binary dim" x="510" y="45">0</text>
    <text class="binary" x="510" y="70">1</text>
    <text class="binary dim glow" x="510" y="95">1</text>
    <text class="binary" x="510" y="120">0</text>
    <text class="binary dim" x="510" y="145">1</text>
    <text class="binary" x="510" y="170">0</text>
    <text class="binary dim" x="510" y="195">0</text>
    <text class="binary" x="510" y="220">1</text>
    <text class="binary dim" x="510" y="245">1</text>
    <text class="binary" x="510" y="270">0</text>
    <text class="binary dim" x="510" y="295">1</text>
    <text class="binary" x="510" y="320">0</text>
    <text class="binary dim" x="510" y="345">1</text>
    <text class="binary glow" x="510" y="370">1</text>
  </g>
  
  <!-- COLUMN 14 (EVEN - moves DOWN) -->
  <g class="col14">
    <text class="binary" x="550" y="20">0</text>
    <text class="binary dim" x="550" y="45">1</text>
    <text class="binary" x="550" y="70">0</text>
    <text class="binary dim" x="550" y="95">1</text>
    <text class="binary" x="550" y="120">1</text>
    <text class="binary dim" x="550" y="145">0</text>
    <text class="binary" x="550" y="170">1</text>
    <text class="binary dim" x="550" y="195">0</text>
    <text class="binary glow" x="550" y="220">0</text>
    <text class="binary dim" x="550" y="245">1</text>
    <text class="binary" x="550" y="270">0</text>
    <text class="binary dim" x="550" y="295">1</text>
    <text class="binary" x="550" y="320">1</text>
    <text class="binary dim" x="550" y="345">0</text>
    <text class="binary" x="550" y="370">1</text>
  </g>
  
  <!-- COLUMN 15 (ODD - moves UP) -->
  <g class="col15">
    <text class="binary" x="590" y="20">1</text>
    <text class="binary dim" x="590" y="45">1</text>
    <text class="binary" x="590" y="70">0</text>
    <text class="binary dim" x="590" y="95">0</text>
    <text class="binary" x="590" y="120">1</text>
    <text class="binary dim" x="590" y="145">0</text>
    <text class="binary glow" x="590" y="170">1</text>
    <text class="binary dim" x="590" y="195">1</text>
    <text class="binary" x="590" y="220">0</text>
    <text class="binary dim" x="590" y="245">1</text>
    <text class="binary" x="590" y="270">0</text>
    <text class="binary dim" x="590" y="295">0</text>
    <text class="binary" x="590" y="320">1</text>
    <text class="binary dim" x="590" y="345">1</text>
    <text class="binary" x="590" y="370">0</text>
  </g>
  
  <!-- COLUMN 16 (EVEN - moves DOWN) -->
  <g class="col16">
    <text class="binary" x="630" y="20">0</text>
    <text class="binary dim glow" x="630" y="45">1</text>
    <text class="binary" x="630" y="70">1</text>
    <text class="binary dim" x="630" y="95">0</text>
    <text class="binary" x="630" y="120">0</text>
    <text class="binary dim" x="630" y="145">1</text>
    <text class="binary" x="630" y="170">0</text>
    <text class="binary dim" x="630" y="195">1</text>
    <text class="binary" x="630" y="220">1</text>
    <text class="binary dim" x="630" y="245">0</text>
    <text class="binary" x="630" y="270">1</text>
    <text class="binary dim" x="630" y="295">0</text>
    <text class="binary" x="630" y="320">0</text>
    <text class="binary dim" x="630" y="345">1</text>
    <text class="binary" x="630" y="370">1</text>
  </g>
  
  <!-- Extra columns to fill width -->
  <g class="col1">
    <text class="binary" x="670" y="20">1</text>
    <text class="binary dim" x="670" y="45">0</text>
    <text class="binary" x="670" y="70">1</text>
    <text class="binary dim" x="670" y="95">0</text>
    <text class="binary" x="670" y="120">0</text>
    <text class="binary dim" x="670" y="145">1</text>
    <text class="binary" x="670" y="170">1</text>
    <text class="binary dim" x="670" y="195">0</text>
    <text class="binary glow" x="670" y="220">1</text>
    <text class="binary dim" x="670" y="245">0</text>
    <text class="binary" x="670" y="270">1</text>
    <text class="binary dim" x="670" y="295">1</text>
    <text class="binary" x="670" y="320">0</text>
    <text class="binary dim" x="670" y="345">0</text>
    <text class="binary" x="670" y="370">1</text>
  </g>
  
  <g class="col2">
    <text class="binary" x="710" y="20">0</text>
    <text class="binary dim" x="710" y="45">1</text>
    <text class="binary" x="710" y="70">0</text>
    <text class="binary dim" x="710" y="95">1</text>
    <text class="binary" x="710" y="120">1</text>
    <text class="binary dim" x="710" y="145">0</text>
    <text class="binary" x="710" y="170">0</text>
    <text class="binary dim" x="710" y="195">1</text>
    <text class="binary" x="710" y="220">0</text>
    <text class="binary dim" x="710" y="245">1</text>
    <text class="binary glow" x="710" y="270">1</text>
    <text class="binary dim" x="710" y="295">0</text>
    <text class="binary" x="710" y="320">1</text>
    <text class="binary dim" x="710" y="345">0</text>
    <text class="binary" x="710" y="370">0</text>
  </g>
  
  <g class="col3">
    <text class="binary" x="750" y="20">1</text>
    <text class="binary dim" x="750" y="45">1</text>
    <text class="binary" x="750" y="70">0</text>
    <text class="binary dim" x="750" y="95">1</text>
    <text class="binary" x="750" y="120">0</text>
    <text class="binary dim" x="750" y="145">0</text>
    <text class="binary" x="750" y="170">1</text>
    <text class="binary dim" x="750" y="195">1</text>
    <text class="binary" x="750" y="220">0</text>
    <text class="binary dim" x="750" y="245">1</text>
    <text class="binary" x="750" y="270">0</text>
    <text class="binary dim glow" x="750" y="295">1</text>
    <text class="binary" x="750" y="320">1</text>
    <text class="binary dim" x="750" y="345">0</text>
    <text class="binary" x="750" y="370">1</text>
  </g>
  
  <g class="col4">
    <text class="binary" x="790" y="20">0</text>
    <text class="binary dim" x="790" y="45">0</text>
    <text class="binary" x="790" y="70">1</text>
    <text class="binary dim" x="790" y="95">1</text>
    <text class="binary" x="790" y="120">0</text>
    <text class="binary dim" x="790" y="145">1</text>
    <text class="binary" x="790" y="170">0</text>
    <text class="binary dim" x="790" y="195">0</text>
    <text class="binary glow" x="790" y="220">1</text>
    <text class="binary dim" x="790" y="245">1</text>
    <text class="binary" x="790" y="270">0</text>
    <text class="binary dim" x="790" y="295">1</text>
    <text class="binary" x="790" y="320">0</text>
    <text class="binary dim" x="790" y="345">1</text>
    <text class="binary" x="790" y="370">1</text>
  </g>
</svg>
