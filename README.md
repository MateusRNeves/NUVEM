<!DOCTYPE html>
<html lang="pt">
<head>
  <meta charset="UTF-8">
  <title>Nuven</title>
  <style>
    :root {
      --clr: #0f0; /* Cor estilo Matrix */
    }

    @keyframes animatecolor {
      0% {
        filter: hue-rotate(0deg);
      }
      100% {
        filter: hue-rotate(360deg);
      }
    }

    body {
      background: #000;
      margin: 0;
      padding: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .conteiner .cloud {
      position: relative;
      width: 300px;
      z-index: 100;
      filter: drop-shadow(0 0 35px var(--clr));
      animation: animatecolor 5s linear infinite;
    }

    .conteiner .cloud h2 {
      position: absolute;
      left: 50%;
      transform: translateX(-50%);
      white-space: nowrap;
      color: transparent;
      font-size: 2em;
      z-index: 1000;
      padding: 0 10px;
      border-radius: 10px;
    }

    .conteiner .cloud h2::before {
      content: '';
      position: absolute;
      top: -115px;
      left: 50%;
      transform: translateX(-50%);
      border-radius: 100px;
      width: 120%;
      height: 100px;
      background: var(--clr);
      opacity: 0.2;
    }
  </style>
</head>
<body>
  <div class="conteiner">
    <div class="cloud">
      <h2>Efeito Chuva Matrix</h2>
    </div>
  </div>

  <script>
    // Aqui você pode colocar código para animar ou gerar o efeito Matrix futuramente
    // Por enquanto, só deixamos o setup visual pronto
  </script>
</body>
</html>