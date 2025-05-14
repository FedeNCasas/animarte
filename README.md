<!DOCTYPE html>

<html lang="es">
<head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>AnimArte San Juan</title>
<style>
    * {margin: 0; padding: 0; box-sizing: border-box;}
    body {
  background: url('paracaidas.jpg') no-repeat center center fixed;
  background-size: cover;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  overflow-x: hidden;
  color: #333;
}
    @keyframes animatedBackground {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
    
header {
  background-color: #ffffff;
  padding: 1rem 2rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: sticky;
  top: 0;
  z-index: 1000;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
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
  color: #ff7f00;
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
    .hero p {
      font-size: 1.2rem;
      margin-bottom: 1.5rem;
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
    .faq summary::before {
      content: '❓ ';
      margin-right: 0.5rem;
      color: #ff7f00;
    }
    .faq[open] summary::before {
      content: '✅ ';
    }
    .faq summary {
      transition: background 0.3s ease, color 0.3s ease;
      padding: 0.5rem;
      border-radius: 8px;
    }
    .faq[open] summary {
      background: #fff7e6;
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
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
    .floating-balloons {
      position: fixed;
      top: 100%;
      left: 0;
      width: 100%;
      height: 0;
      z-index: 0;
      pointer-events: none;
      overflow: visible;
    }
    .balloon {
      position: absolute;
      bottom: -100px;
      width: 40px;
      height: 60px;
      background: radial-gradient(circle at 30% 30%, #ffd1dc, #ff69b4);
      border-radius: 50% 50% 45% 45%;
      animation: floatBalloon 20s linear infinite;
      opacity: 0.7;
    }
    @keyframes floatBalloon {
      0% {
        transform: translateY(0) scale(1);
        opacity: 0.7;
      }
      50% {
        opacity: 1;
      }
      100% {
        transform: translateY(-110vh) scale(1.1);
        opacity: 0;
      }
    }
  
.footer-banner {
  background-color: #ff7f00;
  color: #fff;
  text-align: center;
  padding: 1.5rem;
  font-weight: bold;
  font-size: 1.1rem;
  box-shadow: 0 -2px 6px rgba(0,0,0,0.1);
  animation: fadeIn 1.2s ease-in;
}

.cta-button {
  background: repeating-linear-gradient(
    45deg,
    red, orange 20%, yellow 40%, green 60%, blue 80%, violet 100%
  );
  color: white;
  padding: 1rem 2rem;
  border-radius: 50px;
  text-decoration: none;
  font-weight: bold;
  font-size: 1.1rem;
  box-shadow: 0 3px 6px rgba(0,0,0,0.2);
  transition: all 0.3s ease;
}
.cta-button:hover {
  transform: translateY(-4px) scale(1.07);
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
}

.hero, .testimonials, .faq-section, .footer-banner {
  margin-top: 3rem;
  margin-bottom: 3rem;
}
</style>
<script>
document.addEventListener("DOMContentLoaded", function () {
  const colors = ['#FFD700', '#FF69B4', '#87CEEB', '#32CD32', '#FF7F50'];
  for (let i = 0; i < 100; i++) {
    const confetti = document.createElement("div");
    confetti.classList.add("confetti");
    confetti.style.left = Math.random() * 100 + "vw";
    confetti.style.animationDelay = Math.random() * 5 + "s";
    confetti.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
    document.body.appendChild(confetti);
  }
});
</script>
<style>
.confetti {
  position: fixed;
  top: -10px;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  opacity: 0.8;
  animation: fall 6s linear infinite;
  z-index: 1;
}
@keyframes fall {
  0% {
    transform: translateY(0) rotate(0deg);
    opacity: 1;
  }
  100% {
    transform: translateY(100vh) rotate(360deg);
    opacity: 0;
  }
}
</style>
</head>
<body style="background: url('paracaidas.jpg') no-repeat center center fixed;background-size: cover;font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;overflow-x: hidden;color: #333;">
<header>
<div class="max-w-7xl mx-auto px-4 py-4 flex items-center justify-between">
<!-- Logo a la izquierda -->
<div class="flex-shrink-0">
<img alt="Logo AnimArte" class="h-12 w-auto" src="logo.png"/>
</div>
<!-- Menú centrado -->
<nav class="hidden md:flex gap-6 text-orange-600 font-semibold text-sm md:text-base mx-auto">
<a class="hover:text-pink-500" href="index.html">Inicio</a>
<a class="hover:text-pink-500" href="propuestas.html">Propuestas</a>
<a class="hover:text-pink-500" href="adicionales.html">Adicionales</a>
<a class="hover:text-pink-500" href="quienes-somos.html">Quiénes somos</a>
<a class="hover:text-pink-500" href="contacto.html">Contacto</a>
</nav>
<!-- Redes sociales a la derecha -->
<div class="flex gap-3">
<a href="https://www.instagram.com/s/aGlnaGxpZ2h0OjE3OTg5MjY5NTA2MjE1MTY4" target="_blank">
<img alt="Instagram" class="h-6 w-6" src="https://img.icons8.com/ios-filled/25/E4405F/instagram-new.png"/>
</a>
<a href="https://www.facebook.com/animarte.sanjuan" target="_blank">
<img alt="Facebook" class="h-6 w-6" src="https://img.icons8.com/ios-filled/25/1877F2/facebook-new.png"/>
</a>
</div>
</div>
</header>
<main>
<section class="hero">
<h1>🎉 ¡Bienvenid@ a AnimArte!</h1>
<p>Creamos momentos mágicos que dejan huellas. Somos especialistas en animación infantil con corazón 💛</p>
<a class="cta-button" href="propuestas.html">Conocé nuestras propuestas</a>
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
<a href="https://www.google.com/maps/place/Animarte+San+Juan/@-31.5423433,-68.5578874,17z/data=!4m8!3m7!1s0xa5ded485c2c4507b:0x29665f791757b6cf!8m2!3d-31.5423433!4d-68.5578874!9m1!1b1!16s%2Fg%2F11s59y94l0?hl=es&amp;entry=ttu&amp;authuser=0&amp;review=1" style="display: inline-flex; align-items: center; gap: 0.5rem; background-color: #ff7f00; color: white; padding: 0.9rem 1.8rem; border-radius: 40px; text-decoration: none; font-weight: bold; font-size: 1rem; box-shadow: 0 4px 10px rgba(0,0,0,0.25); transition: transform 0.2s ease-in-out;" target="_blank">
        ⭐ Ver más reseñas reales en Google Maps
        <img alt="Google Maps" height="24" src="https://img.icons8.com/color/48/google-maps-new.png" width="24"/>
</a>
</div>
<section class="faq-section">
<h2>❓ Preguntas Frecuentes</h2>
<details class="faq">
<summary>¿Qué propuesta recomiendan para cada edad?</summary>
<p>Dependiendo de la edad de los niños, recomendamos propuestas específicas que se adaptan a sus intereses y energía. ¡Consultanos para recomendarte la ideal! 🎈</p>
</details>
<details class="faq">
<summary>¿A qué hora conviene comenzar la animación?</summary>
<p>Sugerimos comenzar una hora y media después del inicio del evento para asegurar que estén todos los invitados presentes y listos para disfrutar.</p>
</details>
<details class="faq">
<summary>¿Qué incluye cada propuesta y cada adicional?</summary>
<p>Las propuestas incluyen animación, sonido, banderines, dos profes, dos horas de diversión y mucho más. Los adicionales varían según lo que elijas (maquillaje, globología, slime, etc).</p>
</details>
<details class="faq">
<summary>¿Cuánto cuesta cada adicional?</summary>
<p>El valor depende del adicional. Consultanos por WhatsApp para pasarte el tarifario actualizado.</p>
</details>
<details class="faq">
<summary>¿Viajan a otras localidades como Caucete o Ullum?</summary>
<p>¡Sí! Vamos a muchas zonas de San Juan. Consultanos para saber si llegamos a tu localidad. Si estás fuera del radio de la Circunvalación, se aplica un costo adicional.</p>
</details>
</section>
<div class="footer-banner">
      Empresa familiar con más de 10 años repartiendo sonrisas 💕<br/>
      ¡Gracias por confiar en AnimArte San Juan!
    </div>
</main>
<a class="whatsapp-button" href="https://wa.me/5492645123339?text=Hola,%20me%20interesa%20una%20animación%20para%20mi%20evento%20🥳" target="_blank">
<img alt="WhatsApp" height="30" src="https://img.icons8.com/ios-filled/50/ffffff/whatsapp.png" width="30"/>
</a>
</body>
</html>
