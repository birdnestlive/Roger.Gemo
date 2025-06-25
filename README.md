<!DOCTYPE html>
<html lang="sv">
<head>
  <meta charset="UTF-8" />
  <title>Fågelholk med Talgoxar</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #e0f7fa;
      color: #2c3e50;
      margin: 40px;
      max-width: 700px;
    }
    h1 {
      color: #1b5e20;
      text-align: center;
    }
    img {
      display: block;
      margin: 20px auto;
      max-width: 100%;
      border-radius: 12px;
      box-shadow: 0 0 10px rgba(0,0,0,0.3);
      cursor: pointer;
      animation: float 4s ease-in-out infinite;
    }
    @keyframes float {
      0%, 100% {
        transform: translateY(0);
      }
      50% {
        transform: translateY(-15px);
      }
    }
    p {
      font-size: 1.1em;
      line-height: 1.6em;
    }
    footer {
      margin-top: 40px;
      font-size: 0.9em;
      text-align: center;
      color: #555;
    }
  </style>
</head>
<body>
  <h1>Fågelholk med Talgoxar</h1>
  
  <img id="birdImage" src="https://upload.wikimedia.org/wikipedia/commons/7/7b/Great_Tit_%28Parus_major%29_in_Norway_2015-06-19_01.jpg" alt="Talgoxe på gren" title="Klicka för fågelläte" />

  <p>Talgoxen (Parus major) är en vanlig och välkänd fågel i Sverige som ofta bygger bo i fågelholkar under våren. En fågelholk är en konstgjord bostad som hjälper fåglar att hitta trygga platser för att lägga sina ägg och föda upp sina ungar.</p>

  <p>Genom att sätta upp en fågelholk i trädgården eller på balkongen kan du bidra till att hjälpa talgoxar och andra småfåglar att trivas och föröka sig. Talgoxar är också duktiga på att hålla efter skadeinsekter, vilket är bra för din trädgård!</p>

  <footer>© 2025 Fågelholksentusiasten</footer>

  <audio id="birdSound" src="https://www.xeno-canto.org/sounds/uploaded/RAHSZQOTJM/XC577512-Tit%20munch%20MS%2003-19-20.mp3" preload="auto"></audio>

  <script>
    const birdImage = document.getElementById('birdImage');
    const birdSound = document.getElementById('birdSound');

    birdImage.addEventListener('click', () => {
      birdSound.currentTime = 0;
      birdSound.play();
    });
  </script>
</body>
</html>
