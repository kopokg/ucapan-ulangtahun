<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Selamat Ulang Tahun</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(to bottom, #ffdde1, #ee9ca7);
      color: #fff;
      font-family: 'Segoe UI', sans-serif;
      text-align: center;
      overflow: hidden;
    }
    h1 {
      margin-top: 80px;
      font-size: 2.5em;
      animation: fadeIn 2s ease-in-out;
    }
    p {
      font-size: 1.2em;
      margin: 20px;
      animation: fadeIn 3s ease-in-out;
    }
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
    .butterfly {
      position: absolute;
      width: 50px;
      animation: fly 10s infinite ease-in-out;
    }
    @keyframes fly {
      0% { transform: translateY(0) translateX(0) rotate(0); }
      50% { transform: translateY(-200px) translateX(200px) rotate(180deg); }
      100% { transform: translateY(0) translateX(0) rotate(360deg); }
    }
    .confetti {
      position: absolute;
      width: 5px;
      height: 5px;
      background: white;
      animation: fall 5s linear infinite;
    }
    @keyframes fall {
      0% { top: -10px; opacity: 1; }
      100% { top: 100vh; opacity: 0; }
    }
  </style>
</head>
<body>
  <audio autoplay loop>
    <source src="https://www.bensound.com/bensound-music/bensound-romantic.mp3" type="audio/mp3">
  </audio>

  <h1>Selamat Ulang Tahun!</h1>
  <p>Seperti kupu-kupu yang indah,  
  hadirmu membawa warna dan kehangatan dalam hidup ini.  
  Semoga bahagia dan cinta selalu menyertaimu.  
  Dari seseorang yang diam-diam memperhatikanmu 💕</p>

  <img src="https://i.ibb.co/X3gnz8K/butterfly.png" class="butterfly" style="top:20%; left:10%;">
  <img src="https://i.ibb.co/X3gnz8K/butterfly.png" class="butterfly" style="top:50%; left:70%;">
  <img src="https://i.ibb.co/X3gnz8K/butterfly.png" class="butterfly" style="top:30%; left:40%;">

  <script>
    for (let i = 0; i < 50; i++) {
      let c = document.createElement('div');
      c.className = 'confetti';
      c.style.left = Math.random() * 100 + 'vw';
      c.style.animationDelay = Math.random() * 5 + 's';
      document.body.appendChild(c);
    }
  </script>
</body>
</html>
