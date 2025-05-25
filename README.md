<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<title>Carta para ti 💕</title>
<style>
  body {
    background: linear-gradient(270deg, #ff69b4, #000);
    background-size: 400% 400%;
    animation: gradient 15s ease infinite;
    color: #fff;
    font-family: 'Courier New', monospace;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    padding: 20px;
    text-align: center;
  }
  #texto {
    max-width: 6000px;
    font-size: 100px;
    white-space: pre-wrap;
  }
  @keyframes gradient {
    0%{background-position:0% 50%;}
    50%{background-position:100% 50%;}
    100%{background-position:0% 50%;}
  }
</style>
</head>
<body>
  <div id="texto"></div>
  <script>
    const texto = `Hola mi amor ❤️\n\nCada día a tu lado es magia.\nEres mi sueño hecho realidad.\n\nTe amo mucho. 💕`;
    let i = 0;
    const contenedor = document.getElementById("texto");

    function escribir() {
      if (i < texto.length) {
        contenedor.textContent += texto.charAt(i);
        i++;
        setTimeout(escribir, 80);
      }
    }

    escribir();
  </script>
</body>
</html>
