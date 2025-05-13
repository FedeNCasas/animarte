<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AnimArte San Juan</title>
  <style>
    * {margin: 0; padding: 0; box-sizing: border-box;}
    body {
      background-image: url('/mnt/data/612f4aaf-d6d2-4e17-a993-6f5c81e3ac45.png');
      background-size: cover;
      background-repeat: no-repeat;
      background-attachment: fixed;
      background-position: center;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      /* background gradient eliminado porque ya hay una imagen */
      background-size: 800% 800%;
      animation: animatedBackground 20s ease infinite;
      overflow-x: hidden;
      color: #333;
    }
    @keyframes animatedBackground {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
    header {
      background-color: #ff7f00;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 1000;
    }
    header img {
      height: 60px;
      border-radius: 12px;
      background: white;
      padding: 4px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.2);
      transition: transform 0.3s ease;
    }
    header img:hover {
      transform: scale(1.1);
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
    .hero {
      text-align: center;
      padding: 3rem 1rem;
      background: rgba(255, 255, 255, 0.8);
      border-radius: 16px;
      margin: 2rem auto;
      max-width: 700px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
      animation: fadeIn 1s ease-out;
    }
    .hero h1 {
      font-size: 2.6rem;
      color: #ff7f00;
      margin-bottom: 1rem;
    }
    .hero p {
      font-size: 1.2rem;
      margin-bottom: 1.5rem;
    }
    .cta-button {
      background: linear-gradient(45deg, #ff7f00, #ffcd00);
      color: #fff;
      padding: 1rem 2rem;
      border-radius: 50px;
      text-decoration: none;
      font-weight: bold;
      font-size: 1.1rem;
      box-shadow: 0 3px 6px rgba(0,0,0,0.2);
    }
    .whatsapp-button {
      position: fixed;
      bottom: 20px;
      right: 20px;
      width: 60px;
      height: 60px;
      background: linear-gradient(135deg, #25D366, #128C7E);
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 4px 8px rgba(0,0,0,0.3);
      animation: pulse 2s infinite;
    }
    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.1); }
      100% { transform: scale(1); }
    }
    .faq-section {
      background: #fff;
      padding: 2rem;
      margin: 3rem auto;
      border-radius: 12px;
      max-width: 700px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }
    .faq-section h2 {
      text-align: center;
      margin-bottom: 1rem;
      color: #ff7f00;
    }
    .faq {
      margin-bottom: 1rem;
    }
    .faq summary {
      font-weight: bold;
      cursor: pointer;
      color: #333;
    }
    .faq p {
      margin-top: 0.5rem;
    }
    .testimonials {
      margin: 2rem 1rem;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1rem;
    }
    .testimonial {
      background: #fff;
      padding: 1rem;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      max-width: 280px;
    }
    .testimonial p {
      font-size: 1.1rem;
      font-style: italic;
    }
    .testimonial span {
      font-weight: bold;
      display: block;
      margin-top: 0.5rem;
      color: #ff7f00;
    }
    .footer-banner {
      text-align: center;
      background: #ff7f00;
      color: #fff;
      padding: 2rem 1rem;
      margin-top: 3rem;
      border-radius: 12px 12px 0 0;
      font-size: 1.2rem;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <header>
    <a href="index.html">
      <img src="logo.png" alt="Logo AnimArte" />
    </a>
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
      <p>Creamos momentos mágicos que dejan huellas. Somos especialistas en animación infantil con corazón 💛</p>
      <a href="propuestas.html" class="cta-button">Conocé nuestras propuestas</a>
    </section>

    <div class="testimonials">
      <div class="testimonial">
        <p>“¡Increíble experiencia! Mis hijos se divirtieron como nunca. Súper recomendables.”</p>
        <span>– Mariana G.</span>
      </div>
      <div class="testimonial">
        <p>“Una fiesta llena de magia, juegos y alegría. Gracias AnimArte por tanto amor.”</p>
        <span>– Lucas P.</span>
      </div>
      <div class="testimonial">
        <p>“Todo fue perfecto, desde el primer contacto hasta el cierre del evento.”</p>
        <span>– Carla S.</span>
      </div>
    </div>

    <div style="margin: 2rem 0; text-align: center;">
      <a href="https://www.google.com/maps/place/AnimArte+San+Juan" target="_blank" style="display: inline-flex; align-items: center; gap: 0.5rem; background-color: #ff7f00; color: white; padding: 0.9rem 1.8rem; border-radius: 40px; text-decoration: none; font-weight: bold; font-size: 1rem; box-shadow: 0 4px 10px rgba(0,0,0,0.25); transition: transform 0.2s ease-in-out;">
        ⭐ Ver más reseñas reales en Google Maps
        <img src="https://img.icons8.com/color/48/google-maps-new.png" alt="Google Maps" width="24" height="24" />
      </a>
    </div>

    <section class="faq-section">
      <h2>❓ Preguntas Frecuentes</h2>
      <details class="faq">
        <summary>¿Qué incluye la animación?</summary>
        <p>Juegos, música, maquillaje artístico, globología, y mucho más.</p>
      </details>
      <details class="faq">
        <summary>¿Cuánto dura una fiesta?</summary>
        <p>Nuestras animaciones duran entre 1h30 y 2h, dependiendo del pack elegido.</p>
      </details>
      <details class="faq">
        <summary>¿Trabajan en toda la provincia?</summary>
        <p>¡Sí! AnimArte llega a donde nos necesites dentro de San Juan.</p>
      </details>
    </section>

    <div class="footer-banner">
      Empresa familiar con más de 10 años repartiendo sonrisas 💕<br />
      ¡Gracias por confiar en AnimArte San Juan!
    </div>
  </main>

  <a href="https://wa.me/5492645123339?text=Hola,%20me%20interesa%20una%20animación%20para%20mi%20evento%20🥳" class="whatsapp-button" target="_blank">
    <img src="https://img.icons8.com/ios-filled/50/ffffff/whatsapp.png" alt="WhatsApp" width="30" height="30" />
  </a>
</body>
</html>
