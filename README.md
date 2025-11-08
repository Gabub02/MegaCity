<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Mega City RP — Realistisches GTA Roleplay</title>
  <meta name="description" content="Mega City RP — Cleanes, realistisches GTA V Roleplay. Fair, modern und mit Fokus auf Immersion und Community." />
  <meta name="theme-color" content="#FFD700" />
  <link rel="icon" href="mlogo42.png" type="image/png" />
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            gold: '#FFD700',
            mcblack: '#0b0b0b',
          }
        }
      }
    }
  </script>
  <style>
    html { 
      scroll-behavior: smooth; 
      scroll-padding-top: 80px; /* Wichtig für korrekte Scroll-Position */
    }
    body { 
      overflow-x: hidden; 
      padding-top: 0; /* Header-Höhe ausgleichen */
    }
    .glass { 
      background: rgba(255,255,255,0.05); 
      backdrop-filter: blur(8px); 
    }
    .card { 
      background: rgba(255,255,255,0.03); 
      transition: all 0.3s ease; 
    }
    .card:hover { 
      background: rgba(255,255,255,0.07); 
      transform: translateY(-4px); 
    }
    .glow { 
      text-shadow: 0 0 18px rgba(255,215,0,0.35); 
    }
    .fade-in { 
      opacity: 0; 
      transform: translateY(20px); 
      transition: all 0.8s ease-out; 
    }
    .fade-in.visible { 
      opacity: 1; 
      transform: translateY(0); 
    }
    .bg-animate {
      position: fixed;
      inset: 0;
      background: radial-gradient(circle at 20% 30%, rgba(255,215,0,0.05), transparent 60%), 
                  radial-gradient(circle at 80% 70%, rgba(255,215,0,0.08), transparent 60%);
      animation: moveBg 20s ease-in-out infinite alternate;
      z-index: -1;
    }
    @keyframes moveBg {
      0% { background-position: 0% 0%, 100% 100%; }
      100% { background-position: 100% 0%, 0% 100%; }
    }
    
    /* Korrekte Positionierung für Anker-Links */
    section {
      position: relative;
    }
    #features, #about, #rules, #team {
      scroll-margin-top: 80px; /* Gleicht fixed Header aus */
    }
  </style>
</head>
<body class="bg-gradient-to-b from-black via-gray-900 to-mcblack text-gray-100 antialiased relative">

  <div class="bg-animate"></div>

  <!-- HEADER - FIXED PROBLEM -->
  <header id="navbar" class="fixed top-0 left-0 w-full z-50 bg-black/90 backdrop-blur-md border-b border-gray-800 transition-all duration-500">
    <nav class="max-w-6xl mx-auto px-6 py-4 flex items-center justify-between">
      <div class="flex items-center gap-3">
        <img src="mlogo42.png" alt="Mega City RP Logo" class="h-10 w-10 rounded-md object-cover ring-1 ring-gold/30" />
        <div>
          <a href="#hero" class="text-lg font-semibold glow hover:text-gold transition">Mega City RP</a>
          <p class="text-xs text-gray-400 -mt-0.5">Clean · Realistisch · Fair</p>
        </div>
      </div>
      <div class="hidden md:flex gap-8 items-center text-sm">
        <a href="#features" class="hover:text-gold transition py-2">Features</a>
        <a href="regeln.html" class="hover:text-gold transition py-2">Regeln</a>
        <a href="#about" class="hover:text-gold transition py-2">Über uns</a>
        <a href="#team" class="hover:text-gold transition py-2">Team</a>
        <a href="https://discord.gg/pGM8hT8tS6" target="_blank" class="px-4 py-2 border border-gold/40 text-gold rounded-lg hover:bg-gold hover:text-black transition">Discord</a>
      </div>
      <button id="mobileBtn" class="md:hidden p-2 text-xl hover:text-gold transition">☰</button>
    </nav>
    <div id="mobileMenu" class="hidden md:hidden bg-black/95 text-center py-3 border-t border-gray-800">
      <a href="#features" class="block py-3 hover:text-gold transition" onclick="closeMobileMenu()">Features</a>
      <a href="regeln.html" class="block py-3 hover:text-gold transition" onclick="closeMobileMenu()">Regeln</a>
      <a href="#about" class="block py-3 hover:text-gold transition" onclick="closeMobileMenu()">Über uns</a>
      <a href="#team" class="block py-3 hover:text-gold transition" onclick="closeMobileMenu()">Team</a>
      <a href="https://discord.gg/pGM8hT8tS6" target="_blank" class="block py-3 text-gold hover:text-yellow-300 transition">Discord</a>
    </div>
  </header>

  <!-- HERO - MIT PADDING TOP FÜR FIXED HEADER -->
  <section id="hero" class="min-h-screen flex flex-col justify-center items-center text-center px-6 pt-20">
    <h1 class="text-5xl md:text-7xl font-extrabold tracking-tight mb-4 glow fade-in">Mega City RP</h1>
    <p class="max-w-2xl text-gray-300 text-lg mb-8 fade-in">Tauche ein in eine lebendige Stadt voller Geschichten, Emotionen und realistischem RP.  
      Dein Abenteuer beginnt hier — fair, clean & immersiv.</p>
    <div class="flex flex-wrap justify-center gap-4 fade-in">
      <a href="regeln.html" class="px-6 py-3 bg-gold text-black font-semibold rounded-lg hover:bg-yellow-400 transition">Regelwerk</a>
      <a href="https://discord.gg/pGM8hT8tS6" target="_blank" class="px-6 py-3 border border-gold/40 rounded-lg hover:bg-gold/10 transition">Discord</a>
    </div>
  </section>

  <!-- FEATURES -->
  <section id="features" class="py-20 px-6 border-t border-gray-800 fade-in">
    <div class="max-w-6xl mx-auto text-center">
      <h2 class="text-3xl font-bold mb-10 glow">Was macht uns besonders?</h2>
      <div class="grid md:grid-cols-3 gap-6">
        <div class="card p-6 rounded-lg">
          <h3 class="text-xl font-semibold mb-2 text-gold">Realismus</h3>
          <p class="text-gray-400 text-sm">Alle Interaktionen basieren auf glaubwürdigem Verhalten — kein Power- oder Fail-RP.</p>
        </div>
        <div class="card p-6 rounded-lg">
          <h3 class="text-xl font-semibold mb-2 text-gold">Community</h3>
          <p class="text-gray-400 text-sm">Ein respektvolles, erwachsenes Umfeld mit Fokus auf Qualität statt Quantität.</p>
        </div>
        <div class="card p-6 rounded-lg">
          <h3 class="text-xl font-semibold mb-2 text-gold">Performance</h3>
          <p class="text-gray-400 text-sm">Optimierte Scripts, stabile Server und konstante Weiterentwicklung für flüssiges RP.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- ABOUT -->
  <section id="about" class="py-20 px-6 border-t border-gray-800 fade-in">
    <div class="max-w-5xl mx-auto text-center">
      <h2 class="text-3xl font-bold mb-4 glow">Über uns</h2>
      <p class="text-gray-300 leading-relaxed">Mega City RP ist ein moderner GTA V Roleplay-Server, der Realismus und Freiheit perfekt kombiniert.  
        Unsere Philosophie: faire Regeln, erwachsene Spieler und eine Stadt, die niemals schläft.</p>
    </div>
  </section>

  <!-- RULES (Short) -->
  <section id="rules" class="py-20 px-6 border-t border-gray-800 fade-in">
    <div class="max-w-6xl mx-auto">
      <h2 class="text-3xl font-bold mb-6 glow text-center">Regelwerk (Kurzfassung)</h2>
      <div class="grid md:grid-cols-3 gap-6">
        <aside class="card p-6 rounded-lg">
          <h3 class="font-semibold mb-3">Schnell-Infos</h3>
          <ul class="space-y-2 text-gray-300 text-sm">
            <li>Sprache: Deutsch</li>
            <li>Mindestalter: 18+</li>
            <li>NLR: 30 Minuten</li>
            <li>Max. Crime-Teamgröße: 4</li>
          </ul>
        </aside>
        <div class="md:col-span-2 card p-6 rounded-lg text-gray-300 space-y-4 text-sm leading-relaxed">
          <p><strong>Respekt & Realismus:</strong> Sei fair, glaubwürdig und respektvoll. Keine Beleidigungen, kein Power-/Fail-RP.</p>
          <p><strong>RP-Grundlagen:</strong> NLR gilt 30 Minuten. Kein RDM, kein VDM. Jede Aktion braucht RP-Grundlage.</p>
          <p><strong>Technik & Kommunikation:</strong> Mic-Pflicht, keine Makros, keine Exploits. Supportfälle nur mit Videobeweis.</p>
          <p><em>Für das vollständige Regelwerk klicke auf "Regelwerk" oben oder den Button unten.</em></p>
          <div class="mt-4">
            <a href="regeln.html" class="px-4 py-2 bg-gold text-black rounded-lg font-semibold hover:bg-yellow-400 transition">Zum vollständigen Regelwerk</a>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- TEAM -->
  <section id="team" class="py-20 px-6 border-t border-gray-800 fade-in">
    <div class="max-w-6xl mx-auto text-center">
      <h2 class="text-3xl font-bold mb-10 glow">Team & Kontakt</h2>
      <div class="grid md:grid-cols-3 gap-6">
        <div class="card p-6 rounded-lg">
          <h3 class="font-semibold mb-2 text-gold">Leitung</h3>
          <p class="text-gray-400 text-sm">Kontakt über Discord</p>
        </div>
        <div class="card p-6 rounded-lg">
          <h3 class="font-semibold mb-2 text-gold">Support</h3>
          <p class="text-gray-400 text-sm">Ticket-System im Discord</p>
        </div>
        <div class="card p-6 rounded-lg">
          <h3 class="font-semibold mb-2 text-gold">Technik</h3>
          <p class="text-gray-400 text-sm">Server-IP: <span class="text-gold">mega.city</span></p>
        </div>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer class="border-t border-gray-800 py-10 text-center text-gray-500 text-sm bg-black/60">
    <p>© <span id="year"></span> Mega City RP • Alle Rechte vorbehalten • <a href="https://discord.gg/pGM8hT8tS6" class="hover:text-gold transition">Discord</a></p>
  </footer>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
    
    // Mobile Menu Funktionen
    document.getElementById('mobileBtn').addEventListener('click', () => {
      document.getElementById('mobileMenu').classList.toggle('hidden');
    });
    
    function closeMobileMenu() {
      document.getElementById('mobileMenu').classList.add('hidden');
    }
    
    // Scroll fade-in
    const observer = new IntersectionObserver(entries => {
      entries.forEach(e => {
        if (e.isIntersecting) e.target.classList.add('visible');
      });
    }, { threshold: 0.12 });
    
    document.querySelectorAll('.fade-in').forEach(el => observer.observe(el));
    
    // Navbar scroll behavior
    const navbar = document.getElementById('navbar');
    let lastScrollY = window.scrollY;
    
    window.addEventListener('scroll', () => {
      if (window.scrollY > 50) {
        navbar.classList.add('bg-black/95', 'shadow-lg');
      } else {
        navbar.classList.remove('bg-black/95', 'shadow-lg');
      }
      
      // Hide navbar when scrolling down, show when scrolling up
      if (window.scrollY > lastScrollY && window.scrollY > 200) {
        navbar.style.transform = 'translateY(-100%)';
      } else {
        navbar.style.transform = 'translateY(0)';
      }
      lastScrollY = window.scrollY;
    });
    
    // Smooth scroll for anchor links
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
          target.scrollIntoView({
            behavior: 'smooth',
            block: 'start'
          });
        }
      });
    });
  </script>
</body>
</html>
