<svg xmlns="http://www.w3.org/2000/svg" width="500" height="200" viewBox="0 0 500 200" style="background-color: #000000;">
  <defs>
    <style>
      @keyframes fallDown {
        0% { transform: translateY(-50px); opacity: 0; }
        10% { opacity: 1; }
        90% { opacity: 1; }
        100% { transform: translateY(150px); opacity: 0; }
      }
      @keyframes riseUp {
        0% { transform: translateY(150px); opacity: 0; }
        10% { opacity: 1; }
        90% { opacity: 1; }
        100% { transform: translateY(-50px); opacity: 0; }
      }
      
      /* Odd columns (1,3,5,7) - Move UP */
      .col1 { animation: riseUp 4s infinite; animation-delay: 0s; }
      .col3 { animation: riseUp 4s infinite; animation-delay: 1s; }
      .col5 { animation: riseUp 4s infinite; animation-delay: 2s; }
      .col7 { animation: riseUp 4s infinite; animation-delay: 3s; }
      
      /* Even columns (2,4,6,8) - Move DOWN */
      .col2 { animation: fallDown 4s infinite; animation-delay: 0.5s; }
      .col4 { animation: fallDown 4s infinite; animation-delay: 1.5s; }
      .col6 { animation: fallDown 4s infinite; animation-delay: 2.5s; }
      .col8 { animation: fallDown 4s infinite; animation-delay: 3.5s; }
      
      .binary {
        font-family: 'Courier New', monospace;
        font-size: 14px;
        fill: #00ff00;
      }
      
      .dim {
        opacity: 0.3;
      }
      
      .bright {
        opacity: 1;
        fill: #ffffff;
      }
      
      @keyframes blink {
        0%, 100% { opacity: 1; }
        50% { opacity: 0.5; }
      }
      
      .cursor {
        animation: blink 1s infinite;
      }
    </style>
  </defs>
  
  <!-- Background -->
  <rect width="500" height="200" fill="#000000" rx="5"/>
  
  <!-- Column 1 (ODD - moves UP) -->
  <text class="binary col1" x="20" y="30">1</text>
  <text class="binary col1 dim" x="20" y="50">0</text>
  <text class="binary col1" x="20" y="70">1</text>
  <text class="binary col1 dim" x="20" y="90">1</text>
  <text class="binary col1" x="20" y="110">0</text>
  
  <!-- Column 2 (EVEN - moves DOWN) -->
  <text class="binary col2" x="60" y="30">0</text>
  <text class="binary col2 dim" x="60" y="50">1</text>
  <text class="binary col2" x="60" y="70">0</text>
  <text class="binary col2 dim" x="60" y="90">1</text>
  <text class="binary col2" x="60" y="110">1</text>
  
  <!-- Column 3 (ODD - moves UP) -->
  <text class="binary col3" x="100" y="30">1</text>
  <text class="binary col3 dim" x="100" y="50">1</text>
  <text class="binary col3" x="100" y="70">0</text>
  <text class="binary col3 dim" x="100" y="90">0</text>
  <text class="binary col3" x="100" y="110">1</text>
  
  <!-- Column 4 (EVEN - moves DOWN) -->
  <text class="binary col4" x="140" y="30">0</text>
  <text class="binary col4 dim" x="140" y="50">0</text>
  <text class="binary col4" x="140" y="70">1</text>
  <text class="binary col4 dim" x="140" y="90">0</text>
  <text class="binary col4" x="140" y="110">1</text>
  
  <!-- Column 5 (ODD - moves UP) -->
  <text class="binary col5" x="180" y="30">1</text>
  <text class="binary col5 dim" x="180" y="50">0</text>
  <text class="binary col5" x="180" y="70">1</text>
  <text class="binary col5 dim" x="180" y="90">0</text>
  <text class="binary col5" x="180" y="110">0</text>
  
  <!-- Column 6 (EVEN - moves DOWN) -->
  <text class="binary col6" x="220" y="30">0</text>
  <text class="binary col6 dim" x="220" y="50">1</text>
  <text class="binary col6" x="220" y="70">1</text>
  <text class="binary col6 dim" x="220" y="90">0</text>
  <text class="binary col6" x="220" y="110">1</text>
  
  <!-- Column 7 (ODD - moves UP) -->
  <text class="binary col7" x="260" y="30">1</text>
  <text class="binary col7 dim" x="260" y="50">1</text>
  <text class="binary col7" x="260" y="70">0</text>
  <text class="binary col7 dim" x="260" y="90">1</text>
  <text class="binary col7" x="260" y="110">0</text>
  
  <!-- Column 8 (EVEN - moves DOWN) -->
  <text class="binary col8" x="300" y="30">0</text>
  <text class="binary col8 dim" x="300" y="50">0</text>
  <text class="binary col8" x="300" y="70">1</text>
  <text class="binary col8 dim" x="300" y="90">1</text>
  <text class="binary col8" x="300" y="110">0</text>
  
  <!-- Column 9 (ODD - moves UP) -->
  <text class="binary col1" x="340" y="30">1</text>
  <text class="binary col1 dim" x="340" y="50">0</text>
  <text class="binary col1" x="340" y="70">1</text>
  <text class="binary col1 dim" x="340" y="90">0</text>
  <text class="binary col1" x="340" y="110">1</text>
  
  <!-- Column 10 (EVEN - moves DOWN) -->
  <text class="binary col2" x="380" y="30">1</text>
  <text class="binary col2 dim" x="380" y="50">0</text>
  <text class="binary col2" x="380" y="70">0</text>
  <text class="binary col2 dim" x="380" y="90">1</text>
  <text class="binary col2" x="380" y="110">0</text>
  
  <!-- Column 11 (ODD - moves UP) -->
  <text class="binary col3" x="420" y="30">0</text>
  <text class="binary col3 dim" x="420" y="50">1</text>
  <text class="binary col3" x="420" y="70">1</text>
  <text class="binary col3 dim" x="420" y="90">0</text>
  <text class="binary col3" x="420" y="110">1</text>
  
  <!-- Column 12 (EVEN - moves DOWN) -->
  <text class="binary col4" x="460" y="30">1</text>
  <text class="binary col4 dim" x="460" y="50">0</text>
  <text class="binary col4" x="460" y="70">1</text>
  <text class="binary col4 dim" x="460" y="90">1</text>
  <text class="binary col4" x="460" y="110">0</text>
  
  <!-- Counter Box Overlay -->
  <rect x="150" y="130" width="200" height="50" fill="#000000" stroke="#00ff00" stroke-width="1" rx="3" opacity="0.9"/>
  <text x="250" y="155" font-family="'Courier New', monospace" font-size="16" fill="#00ff00" text-anchor="middle" class="cursor">▶ PROFILE VISITS: 42</text>
</svg>
