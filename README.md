<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AnimArte San Juan</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: Arial, sans-serif;
      color: #333;
      background: linear-gradient(270deg, #ffecd2, #fcb69f, #fcd5ce, #ffe3e3);
      background-size: 800% 800%;
      animation: animatedBackground 20s ease infinite;
      overflow-x: hidden;
    }
    @keyframes animatedBackground {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
    header {
      background-color: #ff7f00;
      color: white;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 1000;
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
    .whatsapp-button {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: linear-gradient(135deg, #25D366, #128C7E);
      background-size: 400% 400%;
      animation: gradientMove 5s ease infinite;
      color: white;
      border: none;
      border-radius: 50%;
      width: 60px;
      height: 60px;
      font-size: 30px;
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 4px 8px rgba(0,0,0,0.3);
      cursor: pointer;
      text-decoration: none;
      z-index: 100;
    }
    @keyframes gradientMove {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
    .whatsapp-button:hover {
      transform: scale(1.1);
    }
    .cta-button {
      display: inline-block;
      margin: 2rem auto;
      padding: 1rem 2rem;
      font-size: 1.2rem;
      color: white;
      background: linear-gradient(45deg, #ff7f00, #ffcd00);
      border: none;
      border-radius: 50px;
      text-decoration: none;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
      cursor: pointer;
      transition: transform 0.3s ease;
    }
    .cta-button:hover {
      transform: scale(1.05);
    }
    .hero {
      text-align: center;
      margin-top: 5rem;
      padding: 2rem;
      background: rgba(255, 255, 255, 0.7);
      border-radius: 16px;
      max-width: 700px;
      margin-left: auto;
      margin-right: auto;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
      animation: fade-in 1s ease-out;
    }
    .hero h1 {
      font-size: 2.8rem;
      color: #ff7f00;
      animation: slide-in 1s ease forwards;
    }
    .hero p {
      font-size: 1.2rem;
      margin-top: 1rem;
      margin-bottom: 1rem;
    }
    @keyframes fade-in {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
    @keyframes slide-in {
      from { opacity: 0; transform: scale(0.9); }
      to { opacity: 1; transform: scale(1); }
    }
    .google-reviews {
      text-align: center;
      margin-top: 3rem;
      padding: 1rem;
    }
    .google-reviews iframe {
      width: 100%;
      max-width: 600px;
      height: 500px;
      border: none;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    }
  </style>
</head>
<body>
  <header>
    <div>
      <a href="index.html">
        <img src="logo.png" alt="Logo AnimArte" style="height: 60px; border-radius: 12px; box-shadow: 0 2px 5px rgba(0,0,0,0.2); transition: transform 0.3s; background: white; padding: 4px;" onmouseover="this.style.transform='scale(1.1)'" onmouseout="this.style.transform='scale(1)'" />
      </a>
    </div>
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
    <section class="hero">
      <h1>🎉 ¡Bienvenid@ a AnimArte!</h1>
      <p>Somos especialistas en hacer de cada evento una experiencia inolvidable. Juegos, creatividad y alegría para todas las edades.</p>
      <a href="propuestas.html" class="cta-button">Elegí tu propuesta</a>
    </section>

    <section class="google-reviews">
      <h2 style="font-size: 1.8rem; color: #ff7f00; margin-bottom: 1rem;">⭐ Lo que dicen nuestras familias</h2>
      <iframe src="https://www.google.com/maps/embed?pb=!4v1715712230996!6m8!1m7!1sCAoSLEFGMVFpcE1XcTRvdFhqRlVjWlQ5NnRfNnRlX3dYZkU0UGktU05GQV9KVFRJ!2m2!1d-31.5383004!2d-68.5269756!3f0!4f0!5f0.7820865974627469" title="Reseñas de Google"></iframe>
    </section>
  <section class="google-reviews">
      <h2 style="font-size: 1.8rem; color: #ff7f00; margin-bottom: 1rem;">⭐ Lo que dicen nuestras familias</h2>
      <iframe src="https://www.google.com/maps/embed?pb=!4v1715712230996!6m8!1m7!1sCAoSLEFGMVFpcE1XcTRvdFhqRlVjWlQ5NnRfNnRlX3dYZkU0UGktU05GQV9KVFRJ!2m2!1d-31.5383004!2d-68.5269756!3f0!4f0!5f0.7820865974627469" title="Reseñas de Google"></iframe>
      <div style="margin-top: 2rem; display: flex; flex-wrap: wrap; justify-content: center; gap: 1rem;">
        <div style="background: #fff; padding: 1rem; border-radius: 12px; box-shadow: 0 4px 10px rgba(0,0,0,0.1); max-width: 280px;">
          <p style="font-size: 1.1rem; font-style: italic;">“¡Increíble experiencia! Mis hijos se divirtieron como nunca. Súper recomendables.”</p>
          <p style="font-weight: bold; margin-top: 0.5rem; color: #ff7f00;">– Mariana G.</p>
        </div>
        <div style="background: #fff; padding: 1rem; border-radius: 12px; box-shadow: 0 4px 10px rgba(0,0,0,0.1); max-width: 280px;">
          <p style="font-size: 1.1rem; font-style: italic;">“Una fiesta llena de magia, juegos y alegría. Gracias AnimArte por tanto amor.”</p>
          <p style="font-weight: bold; margin-top: 0.5rem; color: #ff7f00;">– Lucas P.</p>
        </div>
        <div style="background: #fff; padding: 1rem; border-radius: 12px; box-shadow: 0 4px 10px rgba(0,0,0,0.1); max-width: 280px;">
          <p style="font-size: 1.1rem; font-style: italic;">“Todo fue perfecto, desde el primer contacto hasta el cierre del evento.”</p>
          <p style="font-weight: bold; margin-top: 0.5rem; color: #ff7f00;">– Carla S.</p>
        </div>
      </div>
    </section>
  </main>

  <!-- ✅ Botón de WhatsApp flotante -->
  <a href="https://wa.me/5492645123339?text=Hola,%20mas%20informacion%20porfavor,%20nos%20interesa%20contratar%20el%20servicio%20%F0%9F%98%80%F0%9F%98%80" class="whatsapp-button" target="_blank" aria-label="Chatear por WhatsApp">
    <img src="https://img.icons8.com/ios-filled/50/ffffff/whatsapp.png" alt="WhatsApp" style="width: 30px; height: 30px;" />
  </a>
</body>
</html>
