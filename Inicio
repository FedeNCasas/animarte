<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AnimArte San Juan</title>
  <script src="https://cdn.tailwindcss.com">  document.getElementById('menu-overlay').addEventListener('click', () => {
    menu.classList.add('hidden');
    menu.classList.remove('animate-slide-down');
    document.getElementById('menu-overlay').classList.add('hidden');
    menuBtn.textContent = '☰';
    menuBtn.classList.remove('rotate-180');
  });
</script>
  <link rel="icon" type="image/png" href="favicon.png" />
</head>
<body class="bg-gradient-to-br from-yellow-100 via-pink-100 to-orange-100 min-h-screen overflow-x-hidden">

  <!-- ENCABEZADO CON LOGO Y MENÚ -->
  <header class="w-full fixed top-0 bg-white/80 backdrop-blur-sm shadow z-50">
  <div class="max-w-7xl mx-auto flex justify-between items-center px-4 py-3">
    <img src="/mnt/data/Diseño sin título.pdf" alt="Logo AnimArte" class="h-12 w-auto"/>
    <!-- Botón hamburguesa -->
    <button id="menu-btn" class="md:hidden text-orange-600 text-3xl transition-transform duration-300 transform">☰</button>
    <!-- Menú de navegación -->
    <nav id="menu" class="hidden md:flex flex-col md:flex-row md:items-center gap-4 text-sm md:text-base font-semibold text-orange-600">
      <a href="/" class="hover:text-pink-500">Inicio</a>
      <a href="/propuestas" class="hover:text-pink-500">Propuestas</a>
      <a href="/adicionales" class="hover:text-pink-500">Adicionales</a>
      <a href="/quienes-somos" class="hover:text-pink-500">Quiénes somos</a>
      <a href="/galeria" class="hover:text-pink-500">Galería</a>
      <a href="/packs" class="hover:text-pink-500">Packs</a>
      <a href="/contacto" class="hover:text-pink-500">Contacto</a>
      <a href="https://wa.me/5492645123339" target="_blank" class="hover:text-green-600">WhatsApp</a>
      <a href="https://www.instagram.com/s/aGlnaGxpZ2h0OjE3OTg5MjY5NTA2MjE1MTY4" target="_blank" class="hover:text-pink-700">Instagram</a>
      <a href="https://www.facebook.com/animarte.sanjuan" target="_blank" class="hover:text-blue-600">Facebook</a>
    </nav>
  </div>
  <audio id="menu-sound" src="https://cdn.pixabay.com/audio/2022/03/15/audio_9c5066f49e.mp3"></audio>
<script>
  const menuSound = document.getElementById('menu-sound');
  const menuBtn = document.getElementById('menu-btn');
  const menu = document.getElementById('menu');
  const menuLinks = menu.querySelectorAll('a');

  menuBtn.addEventListener('click', () => {
    menuSound.currentTime = 0;
    menuSound.play();
  const overlay = document.getElementById('menu-overlay');
  overlay.classList.toggle('hidden');
    menu.classList.toggle('hidden');
    menu.classList.toggle('animate-slide-down');
    menuBtn.classList.toggle('rotate-180');
    menuBtn.textContent = menu.classList.contains('hidden') ? '☰' : '✖';
  });

  menuLinks.forEach(link => {
    const menuSound = document.getElementById('menu-sound');
  link.addEventListener('click', () => {
    if (window.innerWidth < 768) {
      menu.classList.add('hidden');
      menu.classList.remove('animate-slide-down');
      document.getElementById('menu-overlay').classList.add('hidden');
      menuBtn.textContent = '☰';
      menuBtn.classList.remove('rotate-180');
    }
  });
});
  });
</script>
<style>
  @keyframes slide-down {
    0% { opacity: 0; transform: translateY(-20px); }
    100% { opacity: 1; transform: translateY(0); }
  }
  .animate-slide-down {
    animation: slide-down 0.3s ease-out;
    background-color: rgba(255, 255, 255, 0.95);
    padding: 1rem;
    border-radius: 0.5rem;
    position: absolute;
    top: 60px;
    right: 20px;
    box-shadow: 0 10px 15px rgba(0,0,0,0.1);
    z-index: 999;
  }
</style>
<div id="menu-overlay" class="hidden fixed inset-0 bg-black/50 z-40"></div>
</header>

  <!-- HERO PRINCIPAL -->
  <section class="pt-24 pb-16 px-6 flex flex-col items-center text-center animate-fade-in">
    <img src="/mnt/data/297741195_6017047334977996_5275350838111807804_n.jpg" alt="Niños jugando" class="w-full max-w-4xl rounded-xl shadow-xl mb-6">
    <h1 class="text-4xl md:text-5xl font-extrabold text-orange-500 mb-4">¡Donde la alegría cobra vida! 🎉</h1>
    <p class="text-lg text-gray-700 mb-6">Animaciones recreativas para infancias inolvidables.</p>
    <audio id="cta-sound" src="https://cdn.pixabay.com/audio/2022/10/26/audio_591fe12aa3.mp3"></audio>

<script>
  const ctaSound = document.getElementById('cta-sound');
  const ctaButton = document.querySelector('a[href="/propuestas.html"]');
  ctaButton.addEventListener('click', () => {
    ctaSound.currentTime = 0;
    ctaSound.play();
  });
</script>
  </section>

  <!-- BOTÓN FLOTANTE DE WHATSAPP -->
  <a href="https://wa.me/5492645123339?text=Hola,%20más%20información%20por%20favor,%20nos%20interesa%20contratar%20el%20servicio%20😀😀"
     target="_blank"
     class="fixed bottom-4 right-4 z-50 bg-gradient-to-br from-green-400 via-yellow-300 to-pink-400 p-4 rounded-full shadow-lg animate-pulse hover:scale-105 transition">
    <img src="https://img.icons8.com/ios-filled/30/ffffff/whatsapp.png" alt="WhatsApp" />
  </a>

  <!-- ANIMACIÓN FADE-IN -->
  <style>
    @keyframes fade-in {
      0% { opacity: 0; transform: translateY(30px); }
      100% { opacity: 1; transform: translateY(0); }
    }
    .animate-fade-in {
      animation: fade-in 1.2s ease-out both;
    }
  </style>

<script>
  document.querySelectorAll('a[href*="reservar"]').forEach(btn => {
    btn.addEventListener('click', () => {
      const ctaSound = document.getElementById('cta-sound');
      if (ctaSound) {
        ctaSound.currentTime = 0;
        ctaSound.play();
      }
    });
  });
</script>
</body>
</html>
