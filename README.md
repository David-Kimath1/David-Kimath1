<svg xmlns="http://www.w3.org/2000/svg" width="400" height="120" viewBox="0 0 400 120">
  <defs>
    <style>
      @keyframes slideUp {
        0% { transform: translateY(0); opacity: 0; }
        10% { opacity: 1; }
        90% { opacity: 1; }
        100% { transform: translateY(-30px); opacity: 0; }
      }
      @keyframes slideDown {
        0% { transform: translateY(0); opacity: 0; }
        10% { opacity: 1; }
        90% { opacity: 1; }
        100% { transform: translateY(30px); opacity: 0; }
      }
      .line1, .line3, .line5 { animation: slideUp 3s infinite; }
      .line2, .line4, .line6 { animation: slideDown 3s infinite; }
      .line1 { animation-delay: 0s; }
      .line2 { animation-delay: 0.5s; }
      .line3 { animation-delay: 1s; }
      .line4 { animation-delay: 1.5s; }
      .line5 { animation-delay: 2s; }
      .line6 { animation-delay: 2.5s; }
      
      @keyframes glow {
        0% { text-shadow: 0 0 5px #00ff00; }
        100% { text-shadow: 0 0 20px #00ff00; }
      }
      .counter-text {
        font-family: 'Courier New', monospace;
        font-size: 32px;
        fill: #00ff00;
        animation: glow 1s ease-in-out infinite alternate;
      }
      .label {
        font-family: 'Courier New', monospace;
        font-size: 14px;
        fill: #00ff00;
        opacity: 0.8;
      }
      .bg {
        fill: #0a0a0a;
        stroke: #00ff00;
        stroke-width: 1;
      }
    </style>
  </defs>
  
  <!-- Background -->
  <rect class="bg" x="0" y="0" width="400" height="120" rx="5" ry="5"/>
  
  <!-- Animated code lines (odd lines go UP, even lines go DOWN) -->
  <text class="line1" x="15" y="50" font-family="monospace" font-size="10" fill="#00ff00" opacity="0.6">const views = 42;</text>
  <text class="line2" x="15" y="65" font-family="monospace" font-size="10" fill="#00ff00" opacity="0.6">function trackVisitor() {</text>
  <text class="line3" x="15" y="80" font-family="monospace" font-size="10" fill="#00ff00" opacity="0.6">  profile.counter++;</text>
  <text class="line4" x="15" y="95" font-family="monospace" font-size="10" fill="#00ff00" opacity="0.6">  return views;</text>
  <text class="line5" x="15" y="110" font-family="monospace" font-size="10" fill="#00ff00" opacity="0.6">}</text>
  <text class="line6" x="15" y="125" font-family="monospace" font-size="10" fill="#00ff00" opacity="0.6">// SYSTEM ACTIVE</text>
  
  <!-- Counter display -->
  <text class="label" x="250" y="40">PROFILE ACCESS COUNT</text>
  <text class="counter-text" x="250" y="85" font-weight="bold">[ 42 ]</text>
  <text class="label" x="250" y="105">LIFETIME VISITS</text>
</svg>
