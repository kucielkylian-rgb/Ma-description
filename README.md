<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Ma Présentation</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500&display=swap" rel="stylesheet">
  <style>
    /* Style général */
    body {
      margin: 0;
      padding: 0;
      font-family: 'Orbitron', sans-serif;
      background: linear-gradient(-45deg, #0f0c29, #302b63, #24243e);
      background-size: 400% 400%;
      animation: gradient 12s ease infinite;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      color: #fff;
      overflow: hidden;
    }

    body::before {
  content: "";
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: radial-gradient(ellipse at bottom, #00f0ff 0%, #001f33 40%, #000000 100%);
  animation: blueFlames 4s infinite ease-in-out alternate;
  z-index: -1;
  filter: blur(1.5px) brightness(1.3);
  opacity: 0.9;
}

@keyframes blueFlames {
  0% {
    transform: scale(1) translateY(0);
    filter: blur(1px) brightness(1.1);
  }
  100% {
    transform: scale(1.05) translateY(-10px);
    filter: blur(2px) brightness(1.4);
  }
}


    @keyframes gradient {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

     .bio-desc {
  background-color: #0f1b2a;
  color: #e0f7ff;
  border: 2px solid #00f0ff;
  padding: 20px;
  border-radius: 12px;
  box-shadow:
    0 0 5px #0f4246,
    0 0 10px #00f0ff,
    0 0 20px #00f0ff,
    0 0 40px #f3f5f5;
  font-size: 1.1em;
  max-width: 600px;
  margin: 30px auto;
  text-align: center;
  font-family: 'Segoe UI', sans-serif;
}

    .bio-card {
      background: rgba(0, 0, 0, 0.7);
      border: 2px solid #00ffe0;
      border-radius: 20px;
      padding: 30px;
      max-width: 500px;
      width: 90%;
      text-align: center;
      box-shadow: 0 0 30px #00ffff;
      animation: fadeIn 1.5s ease;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: scale(0.95); }
      to   { opacity: 1; transform: scale(1); }
    }

    .bio-image img {
      width: 100%;
      border-radius: 20px;
      box-shadow: 0 0 15px #fff;
      margin-bottom: 20px;
    }

    h1 {
      font-size: 2rem;
      margin-bottom: 10px;
      color: #00ffe0;
    }

    .bio-desc {
      font-size: 1rem;
      margin: 15px 0;
      color: #0ce4f3;
    }

    #ambianceBtn {
      background-color: #00ffe0;
      color: #000;
      padding: 12px 24px;
      border: none;
      border-radius: 10px;
      font-weight: bold;
      cursor: pointer;
      transition: all 0.3s ease;
      margin-top: 15px;
    }

    #ambianceBtn:hover {
      background-color: #00bfa5;
      transform: scale(1.05);
    }

    audio {
      display: none;
    }
  </style>
</head>
<body>

  <div class="bio-card">
    <div class="bio-image">
      <!-- 🔥 Mets ici ton image -->
      <img src="c:\Users\PC\Pictures\Screenshots\image_r1k-MxWN_1756119466496_512.webp" alt="Mon personnage stylé">
    </div>

    <h1>𝔖𝔱𝔦𝔠𝔙𝔲𝔦𝔩𝔡𝔢𝔯</h1>
    <p class="bio-desc">
      <!-- ✏️ Ta description ici -->
      Je suis un créateur de site html,
      j'apprend a faire du language Python. Je joue a toute sorte de jeu video je suis quelqu'un comme tout les autres.
       Je fait des dessins sur des plateformes comme Openart.
        J'ai appris a coder grace à Lemoustik suivez le !
    </p>
    <button id="ambianceBtn">🎵 Mettre de l'ambiance</button>
    <audio id="music" src="musique/For Tommorow by @TheManBeHisLa Lyrics.mp3"></audio>
  </div>

  <script>
    // 🎶 Lancer la musique avec le bouton
    const btn = document.getElementById('ambianceBtn');
    const music = document.getElementById('music');

    btn.addEventListener('click', () => {
      music.play();
      btn.textContent = "🎶 Ambiance lancée !";
      btn.disabled = true;
      btn.style.opacity = 0.7;
    });
  </script>

</body>
</html>

