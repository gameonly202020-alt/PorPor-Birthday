# PorPor-Birthday
 <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Por Por's Birthday Party!</title>
  <style>
    body {
      font-family: 'Comic Sans MS', cursive, sans-serif;
      background: linear-gradient(to bottom right, #ffe6f0, #ffccf2);
      color: #d63384;
      text-align: center;
      margin: 0;
      padding: 0;
      overflow-x: hidden;
    }
    .container {
      padding: 20px;
    }
    h1 {
      font-size: 2.8em;
      margin-top: 30px;
      animation: bounce 1.5s infinite;
    }
    @keyframes bounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }
    p {
      font-size: 1.2em;
      margin: 10px 0;
    }
    .photo {
      width: 250px;
      height: 250px;
      border-radius: 50%;
      object-fit: cover;
      border: 5px solid #ff99cc;
      margin: 20px 0;
    }
    .invite-box {
      background: #fff0f5;
      border: 3px dashed #ff66b2;
      border-radius: 15px;
      padding: 20px;
      display: inline-block;
      margin-top: 20px;
      box-shadow: 0 0 15px rgba(255, 102, 178, 0.5);
    }
    .footer {
      margin-top: 30px;
      font-size: 0.9em;
      color: #a30057;
    }
    /* Confetti animation */
    .confetti {
      position: fixed;
      width: 10px;
      height: 10px;
      background: #ff66b2;
      top: 0;
      animation: fall 5s linear infinite;
    }
    @keyframes fall {
      0% { transform: translateY(0) rotate(0deg); }
      100% { transform: translateY(100vh) rotate(360deg); }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>🎉 Por Por's Birthday! 🎉</h1>
    <img src="por_por_photo.jpg" alt="Por Por's Photo" class="photo">
    <div class="invite-box">
      <p><strong>When:</strong> January 1, 2026, 4:30 PM</p>
      <p><strong>Where:</strong> House No. 9G, Prek Pra, Chbar Ampov, Phnom Penh</p>
      <p>Come join us for fun, games, and cake! 🎂</p>
    </div>
    <div class="footer">
      We can’t wait to celebrate with you! 💖
    </div>
  </div>

  <!-- Confetti elements -->
  <script>
    for(let i=0;i<100;i++){
      let confetti = document.createElement('div');
      confetti.className = 'confetti';
      confetti.style.left = Math.random()*100 + 'vw';
      confetti.style.background = hsl(${Math.random()*360}, 100%, 75%);
      confetti.style.animationDuration = (2+Math.random()*3)+'s';
      document.body.appendChild(confetti);
    }
  </script>
</body>
</html>
