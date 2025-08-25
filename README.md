<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <title>Musique d'Ambiance</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      height: 100%;
      font-family: Arial, sans-serif;
      overflow: auto;
    }

    /* Image de fond pleine page */
    body {
      background: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1920&q=80') no-repeat center center fixed;
      background-size: cover;
      position: relative;
      color: white;
    }

    /* Demi-rectangle (petite boîte) centrée horizontalement en haut */
    #musicControl {
      position: fixed; /* fixe sur l'écran */
      top: 10%; /* un peu en dessous du haut */
      left: 50%;
      transform: translateX(-50%);
      width: 50vw; /* largeur moitié de la fenêtre */
      max-width: 600px;
      height: 150px;
      background: rgba(0, 0, 0, 0.7); /* fond noir transparent */
      border-radius: 15px;
      box-shadow: 0 0 20px rgba(255, 165, 0, 0.9);
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 20px;
      z-index: 1000; /* devant tout */
    }

    #musicControl h2 {
      margin-bottom: 20px;
      color: #FFD700;
      font-weight: normal;
      font-size: 1.4rem;
    }

    #ambianceButton {
      background: linear-gradient(45deg, #FFD700, #FFA500);
      border: none;
      border-radius: 30px;
      padding: 12px 40px;
      font-size: 1.2rem;
      color: black;
      cursor: pointer;
      box-shadow: 0 0 15px rgba(255, 165, 0, 0.9);
      transition: transform 0.2s ease;
      user-select: none;
    }

    #ambianceButton:hover {
      transform: scale(1.1);
    }

    /* On cache l'audio */
    audio {
      display: none;
    }
  </style>
</head>
<body>

  <div id="musicControl">
    <h2>Activer la musique d'ambiance</h2>
    <button id="ambianceButton">Démarrer</button>
  </div>

  <audio id="audio" loop>
    <source src="musique/For Tommorow by @TheManBeHisLa Lyrics.mp3" type="audio/mpeg" />
    Ton navigateur ne supporte pas l’audio.
  </audio>

  <script>
    const button = document.getElementById('ambianceButton');
    const musicControl = document.getElementById('musicControl');
    const audio = document.getElementById('audio');

    button.addEventListener('click', () => {
      audio.play();
      musicControl.style.display = 'none'; // Cache la boîte quand musique démarre
    });
  </script>

</body>
</html>

   <audio autoplay loop controls>
  <source src="musique/For Tommorow by @TheManBeHisLa Lyrics.mp3" type="audio/mpeg"/>

</audio>

    

    <style>
        body {
            margin: 0;
            padding: 0;
            background: url('c:https://i.gifer.com/7VE.gif') center center / cover no-repeat;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Arial', sans-serif;
        }

        .main-container {
            text-align: center;
            background-color: rgba(0, 0, 0, 0.5); /* Fond semi-transparent pour lisibilité */
            padding: 30px;
            border-radius: 20px;
        }

        .𝔖𝔱𝔦𝔠𝔙𝔲𝔦𝔩𝔡𝔢𝔯 {
            font-size: 32px;
            color: white;
            text-shadow: 0 0 10px #000;
            margin-bottom: 20px;
        }

        .profile-pic {
            width: 250px;
            height: 250px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid white;
            box-shadow: 0 0 15px rgba(255, 255, 255, 0.6);
        }
    </style>
</head>
<body>
    <div class="main-container">
        <h1 class="𝔖𝔱𝔦𝔠𝔙𝔲𝔦𝔩𝔡𝔢𝔯">𝔖𝔱𝔦𝔠𝔙𝔲𝔦𝔩𝔡𝔢𝔯</h1>
        <img src="95e5d3cd-7b34-496c-83f9-7991815625da.webp" alt="Image de profil" class="profile-pic">
    </div>
</body>
</html>

    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>sticBuilder - Profil</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700&family=Playfair+Display:wght@400;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            cursor: none;
        }

        body {
            overflow: hidden;
            height: 100vh;
            background: radial-gradient(circle at 30% 20%, #FFD700, #FFA500, #FF4500, #8A2BE2, #4B0082, #000080);
            position: relative;
            animation: backgroundShift 8s ease-in-out infinite alternate;
            font-family: 'Playfair Display', serif;
        }

        @keyframes backgroundShift {
            0% { 
                background: radial-gradient(circle at 30% 20%, #FFD700, #FFA500, #FF4500, #8A2BE2, #4B0082, #000080);
            }
            50% {
                background: radial-gradient(circle at 70% 80%, #00BFFF, #1E90FF, #4169E1, #8A2BE2, #DA70D6, #FFB6C1);
            }
            100% { 
                background: radial-gradient(circle at 50% 50%, #FF1493, #FF69B4, #DA70D6, #9370DB, #6A5ACD, #483D8B);
            }
        }

        .main-container {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            text-align: center;
            z-index: 5;
        }

        .username {
            font-family: 'Cinzel', serif;
            font-size: 4rem;
            font-weight: 700;
            color: transparent;
            background: linear-gradient(45deg, #FFD700, #FFA500, #FF4500, #FF1493);
            background-clip: text;
            -webkit-background-clip: text;
            text-shadow: 
                2px 2px 4px rgba(0, 0, 0, 0.5),
                0 0 30px rgba(255, 215, 0, 0.8),
                0 0 60px rgba(255, 69, 0, 0.6);
            animation: textGlow 4s ease-in-out infinite alternate;
            letter-spacing: 0.2em;
            margin-bottom: 30px;
        }

        @keyframes textGlow {
            0% { 
                filter: brightness(1);
                text-shadow: 
                    2px 2px 4px rgba(0, 0, 0, 0.5),
                    0 0 30px rgba(255, 215, 0, 0.8),
                    0 0 60px rgba(255, 69, 0, 0.6);
            }
            100% { 
                filter: brightness(1.3);
                text-shadow: 
                    2px 2px 4px rgba(0, 0, 0, 0.5),
                    0 0 50px rgba(255, 215, 0, 1),
                    0 0 100px rgba(255, 69, 0, 0.8),
                    0 0 150px rgba(255, 20, 147, 0.6);
            }
        }

        .dragon-image {
            width: 400px;
            height: 300px;
            background: linear-gradient(145deg, #E6E6FA, #DDA0DD, #9370DB, #6A5ACD);
            border-radius: 20px;
            margin: 0 auto;
            box-shadow: 
                0 20px 40px rgba(0, 0, 0, 0.3),
                inset 0 0 50px rgba(255, 255, 255, 0.1),
                0 0 100px rgba(138, 43, 226, 0.5);
            animation: imageFloat 6s ease-in-out infinite;
            position: relative;
            overflow: hidden;
            background-image: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 400 300"><text x="50%" y="50%" text-anchor="middle" dy=".3em" fill="rgba(255,255,255,0.8)" font-size="16" font-family="Arial">Remplace par ton image de dragon</text></svg>');
            background-size: cover;
            background-position: center;
            border: 3px solid rgba(255, 215, 0, 0.6);
        }

        @keyframes imageFloat {
            0%, 100% { transform: translateY(0) scale(1); }
            50% { transform: translateY(-10px) scale(1.02); }
        }

        .floating-card {
            position: fixed;
            width: 350px;
            background: rgba(0, 0, 0, 0.85);
            backdrop-filter: blur(15px);
            border: 2px solid rgba(255, 215, 0, 0.6);
            border-radius: 20px;
            padding: 25px;
            color: white;
            box-shadow: 
                0 20px 40px rgba(0, 0, 0, 0.5),
                inset 0 0 50px rgba(255, 215, 0, 0.1);
            pointer-events: none;
            z-index: 1000;
            transition: all 0.1s ease-out;
            transform-origin: top left;
        }

        .card-header {
            display: flex;
            align-items: center;
            gap: 15px;
            margin-bottom: 20px;
            padding-bottom: 15px;
            border-bottom: 1px solid rgba(255, 215, 0, 0.3);
        }

        .profile-pic {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background: linear-gradient(145deg, #FFD700, #FF4500);
            box-shadow: 0 0 20px rgba(255, 215, 0, 0.5);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
            font-weight: bold;
            color: #000;
        }

        .card-title {
            font-family: 'Cinzel', serif;
            font-size: 1.4rem;
            font-weight: 700;
            color: #FFD700;
            margin-bottom: 5px;
        }

        .card-subtitle {
            font-size: 0.9rem;
            color: #DDA0DD;
            opacity: 0.8;
        }

        .card-description {
            font-size: 0.95rem;
            line-height: 1.6;
            color: #E6E6FA;
            margin-bottom: 15px;
        }

        .card-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .tag {
            background: rgba(255, 215, 0, 0.2);
            color: #FFD700;
            padding: 4px 12px;
            border-radius: 15px;
            font-size: 0.8rem;
            border: 1px solid rgba(255, 215, 0, 0.3);
        }

        .magical-particles {
            position: absolute;
            width: 4px;
            height: 4px;
            background: radial-gradient(circle, #FFD700, transparent);
            border-radius: 50%;
            animation: particleFloat 8s linear infinite;
        }

        .magical-particles:nth-child(1) { top: 15%; left: 10%; animation-delay: 0s; }
        .magical-particles:nth-child(2) { top: 25%; right: 20%; animation-delay: 1s; }
        .magical-particles:nth-child(3) { bottom: 30%; left: 15%; animation-delay: 2s; }
        .magical-particles:nth-child(4) { bottom: 40%; right: 10%; animation-delay: 3s; }
        .magical-particles:nth-child(5) { top: 45%; left: 5%; animation-delay: 4s; }
        .magical-particles:nth-child(6) { top: 55%; right: 5%; animation-delay: 5s; }

        @keyframes particleFloat {
            0% { 
                transform: translateY(0) scale(0);
                opacity: 0;
            }
            20% {
                transform: translateY(-20px) scale(1);
                opacity: 1;
            }
            80% {
                transform: translateY(-200px) scale(1);
                opacity: 1;
            }
            100% { 
                transform: translateY(-250px) scale(0);
                opacity: 0;
            }
        }

        .energy-aura {
            position: absolute;
            width: 500px;
            height: 500px;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: radial-gradient(circle, 
                transparent 40%, 
                rgba(255, 215, 0, 0.1) 45%, 
                rgba(255, 69, 0, 0.2) 55%, 
                rgba(138, 43, 226, 0.1) 70%, 
                transparent 80%);
            border-radius: 50%;
            animation: energyPulse 4s ease-in-out infinite;
            z-index: 1;
        }

        @keyframes energyPulse {
            0%, 100% { 
                transform: translate(-50%, -50%) scale(1) rotate(0deg);
                opacity: 0.7;
            }
            50% { 
                transform: translate(-50%, -50%) scale(1.3) rotate(180deg);
                opacity: 1;
            }
        }

        .custom-cursor {
            position: fixed;
            width: 20px;
            height: 20px;
            background: radial-gradient(circle, #FFD700, #FF4500);
            border-radius: 50%;
            pointer-events: none;
            z-index: 9999;
            box-shadow: 0 0 20px #FFD700;
            animation: cursorGlow 2s ease-in-out infinite alternate;
        }

        @keyframes cursorGlow {
            0% { transform: scale(1); }
            100% { transform: scale(1.2); box-shadow: 0 0 30px #FFD700; }
        }

        @media (max-width: 768px) {
            .username {
                font-size: 2.5rem;
            }
            
            .dragon-image {
                width: 300px;
                height: 200px;
            }
            
            .floating-card {
                width: 450px;
                padding: 35px;
            }
            
            * {
                cursor: auto;
            }
        }

        .instructions {
            position: absolute;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            color: rgba(255, 255, 255, 0.7);
            font-size: 0.9rem;
            text-align: center;
            z-index: 10;
        }
    </style>
</head>
<body>
    <div class="energy-aura"></div>
    
    <div class="magical-particles"></div>
    <div class="magical-particles"></div>
    <div class="magical-particles"></div>
    <div class="magical-particles"></div>
    <div class="magical-particles"></div>
    <div class="magical-particles"></div>

    <div class="custom-cursor" id="cursor"></div>

    <div class="main-container">
    <h1 class="𝔖𝔱𝔦𝔠𝔙𝔲𝔦𝔩𝔡𝔢𝔯">𝔖𝔱𝔦𝔠𝔙𝔲𝔦𝔩𝔡𝔢𝔯</h1>
    <img src="c:\Users\PC\Pictures\Screenshots\image_r1k-MxWN_1756119466496_512.webp" alt="Image personnage stylisé" class="image_r1k-MxWN_1756119466496_512">
</div>

<img src="images/95e5d3cd-7b34-496c-83f9-7991815625da.webp" ... >


<img src="c:/Users/PC/Pictures/Screenshots/image_r1k-MxWN_1756119466496_512.webp" alt="Profil" class="profile-pic">




        <div class="card-tags">
            <span class="tag">Développeur</span>
            <span class="tag">Game Designer</span>
            <span class="tag">Artist</span>
            <span class="tag">Creator</span>
        </div>
    </div>

    <div class="floating-card" id="floatingCard">
        <div class="card-header">
            <div class="profile-pic">S</div>
            <div>
                <div class="card-title">sticBuilder</div>
                <div class="card-subtitle">Créateur Légendaire</div>
            </div>
        </div>
        <div class="card-description">
            ✨ Développeur passionné et créateur d'univers magiques<br>
            🎮 Spécialisé dans les jeux interactifs et les expériences immersives<br>
            🐉 Maître des arts numériques et de la programmation créative
        </div>
        <div class="card-tags">
            <span class="tag">Développeur</span>
            <span class="tag">Game Designer</span>
            <span class="tag">Artist</span>
            <span class="tag">Creator</span>
        </div>
    </div>


    <div class="instructions">
        📱 Bougez votre souris ou touchez l'écran • Pour remplacer l'image : changez l'URL dans le CSS
    </div>

    <script>
        const cursor = document.getElementById('cursor');
        const floatingCard = document.getElementById('floatingCard');
        const dragonImage = document.getElementById('dragonImage');
        
        let mouseX = 0;
        let mouseY = 0;
        let cardX = 0;
        let cardY = 0;

        // Suivre la souris
        document.addEventListener('mousemove', (e) => {
            mouseX = e.clientX;
            mouseY = e.clientY;
            
            // Curseur custom
            cursor.style.left = mouseX - 10 + 'px';
            cursor.style.top = mouseY - 10 + 'px';
            
            // Animation fluide pour la carte
            updateCardPosition();
        });

        // Support tactile mobile
        document.addEventListener('touchstart', (e) => {
            if (e.touches[0]) {
                mouseX = e.touches[0].clientX;
                mouseY = e.touches[0].clientY;
                updateCardPosition();
            }
        });

        document.addEventListener('touchmove', (e) => {
            e.preventDefault();
            if (e.touches[0]) {
                mouseX = e.touches[0].clientX;
                mouseY = e.touches[0].clientY;
                updateCardPosition();
            }
        });

        function updateCardPosition() {
            // Position avec offset pour éviter que la carte soit sous le curseur
            const offsetX = 30;
            const offsetY = 30;
            
            cardX = mouseX + offsetX;
            cardY = mouseY + offsetY;
            
            // Vérifier les limites de l'écran
            const cardRect = floatingCard.getBoundingClientRect();
            const maxX = window.innerWidth - cardRect.width - 20;
            const maxY = window.innerHeight - cardRect.height - 20;
            
            if (cardX > maxX) cardX = mouseX - cardRect.width - offsetX;
            if (cardY > maxY) cardY = mouseY - cardRect.height - offsetY;
            if (cardX < 20) cardX = 20;
            if (cardY < 20) cardY = 20;
            
            floatingCard.style.left = cardX + 'px';
            floatingCard.style.top = cardY + 'px';
        }

        // Animation d'apparition progressive
        window.addEventListener('load', () => {
            setTimeout(() => {
                floatingCard.style.opacity = '1';
            }, 500);
        });

        // Initialiser la position
        updateCardPosition();

        // Instructions pour remplacer l'image
        console.log(`
🐉 COMMENT REMPLACER L'IMAGE :

1. Héberge ton image de dragon sur un service comme :
   - Imgur.com
   - Postimg.cc  
   - Ou ton propre serveur

2. Dans le CSS, trouve cette ligne :
   background-image: url('data:image/svg+xml...');

3. Remplace par :
   background-image: url('TON_URL_IMAGE_ICI');

Exemple :
   background-image: url('https://i.imgur.com/tonimage.jpg');

✨ Ton image apparaîtra à la place du placeholder !
        `);
    </script>
</body>
</html>
