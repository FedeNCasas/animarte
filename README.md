<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AnimArte San Juan</title>
  <style>
    body {
      margin: 0;
      font-family: 'Arial', sans-serif;
      background-color: #fff8f0;
      color: #333;
    }
    header {
      background-color: #ff7f00;
      color: white;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    .logo {
      height: 50px;
    }
    nav {
      display: flex;
      gap: 1rem;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }
    nav a:hover {
      text-decoration: underline;
    }
    main {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 80vh;
      text-align: center;
      padding: 2rem;
    }
    h1 {
      font-size: 2.5rem;
      color: #ff7f00;
    }
    p {
      font-size: 1.2rem;
      max-width: 600px;
    }
    .cta-button {
      margin-top: 2rem;
      padding: 1rem 2rem;
      font-size: 1.2rem;
      color: white;
      background: linear-gradient(45deg, #ff7f00, #ffcd00);
      border: none;
      border-radius: 50px;
      text-decoration: none;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    }
    .cta-button:hover {
      transform: scale(1.05);
    }
  </style>
</head>
<body>
  <header>
    <img src="logo.png" alt="Logo AnimArte" class="logo">
    <nav>
      <a href="index.html">Inicio</a>
      <a href="propuestas.html">Propuestas</a>
      <a href="adicionales.html">Adicionales</a>
      <a href="quienes-somos.html">Quiénes somos</a>
      <a href="galeria.html">Galería</a>
      <a href="packs.html">Packs</a>
      <a href="contacto.html">Contacto</a>
    </nav>
  </header>

  <main>
    <h1>¡Bienvenid@ a AnimArte!</h1>
    <p>Somos especialistas en hacer de cada evento una experiencia inolvidable. Juegos, creatividad y alegría para todas las edades.</p>
    <a href="propuestas.html" class="cta-button">Elegí tu propuesta</a>
  </main>
</body>
</html>
