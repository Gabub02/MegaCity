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
            darkgray: '#1a1a1a'
          },
          fontFamily: {
            'heading': ['Inter', 'system-ui', 'sans-serif'],
          }
        }
      }
    }
  </script>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    html { scroll-behavior: smooth; }
    body { overflow-x: hidden; font-family: 'Inter', sans-serif; }
    .glass { background: rgba(255,255,255,0.05); backdrop-filter: blur(12px); border: 1px solid rgba(255,255,255,0.1); }
    .card { background: rgba(255,255,255,0.03); transition: all 0.3s ease; border: 1px solid rgba(255,255,255,0.05); }
    .card:hover { background: rgba(255,255,255,0.07); transform: translateY(-5px); box-shadow: 0 10px 25px rgba(0,0,0,0.2); }
    .glow { text-shadow: 0 0 18px rgba(255,215,0,0.4); }
    .fade-in { opacity: 0; transform: translateY(20px); transition: all 0.8s ease-out; }
    .fade-in.visible { opacity: 1; transform: translateY(0); }
    .bg-animate {
      position: fixed;
      inset: 0;
      background: 
        radial-gradient(circle at 15% 25%, rgba(255,215,0,0.08), transparent 50%), 
        radial-gradient(circle at 85% 75%, rgba(255,215,0,0.06), transparent 50%),
        radial-gradient(circle at 50% 50%, rgba(255,215,0,0.03), transparent 70%);
      animation: moveBg 25s ease-in-out infinite alternate;
      z-index: -1;
    }
    @keyframes moveBg {
      0% { transform: scale(1) rotate(0deg); }
      100% { transform: scale(1.1) rotate(1deg); }
    }
    .gold-gradient {
      background: linear-gradient(135deg, #FFD700 0%, #FFEC8B 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }
    .section-title {
      position: relative;
      display: inline-block;
      margin-bottom: 3rem;
    }
    .section-title:after {
      content: '';
      position: absolute;
      bottom: -10px;
      left: 50%;
      transform: translateX(-50%);
      width: 60px;
      height: 3px;
      background: #FFD700;
      border-radius: 2px;
    }
    .nav-link {
      position: relative;
      padding: 0.5rem 0;
    }
    .nav-link:after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 0;
      width: 0;
      height: 2px;
      background: #FFD700;
      transition: width 0.3s ease;
    }
    .nav-link:hover:after {
      width: 100%;
    }
  </style>
</head>
<body class="bg-gradient-to-b from-black via-gray-900 to-mcblack text-gray-100 antialiased relative">

  <div class="bg-animate"></div>

  <!-- HEADER -->
  <header id="navbar" class="fixed w-full z-50 glass transition-all duration-500">
    <nav class="max-w-7xl mx-auto px-6 py-3 flex items-center justify-between">
      <div class="flex items-center gap-3">
        <img src="mlogo42.png" alt="Mega City RP Logo" class="h-12 w-12 rounded-lg object-cover ring-2 ring-gold/40 shadow-lg" />
        <div>
          <a href="#hero" class="text-xl font-bold gold-gradient">Mega City RP</a>
          <p class="text-xs text-gray-400 -mt-0.5">Clean · Realistisch · Fair</p>
        </div>
      </div>
      <div class="hidden md:flex gap-8 items-center text-sm font-medium">
        <a href="#features" class="nav-link hover:text-gold transition">Features</a>
        <a href="regeln.html" class="nav-link hover:text-gold transition">Regeln</a>
        <a href="#about" class="nav-link hover:text-gold transition">Über uns</a>
        <a href="#team" class="nav-link hover:text-gold transition">Team</a>
        <a href="https://discord.gg/pGM8hT8tS6" target="_blank" class="px-5 py-2.5 bg-gold text-black font-semibold rounded-lg hover:bg-yellow-400 transition shadow-md">Discord</a>
      </div>
      <button id="mobileBtn" class="md:hidden p-2 text-xl hover:text-gold transition">☰</button>
    </nav>
    <div id="mobileMenu" class="hidden md:hidden glass text-center py-4 border-t border-gray-800">
      <a href="#features" class="block py-3 hover:text-gold transition">Features</a>
      <a href="regeln.html" class="block py-3 hover:text-gold transition">Regeln</a>
      <a href="#about" class="block py-3 hover:text-gold transition">Über uns</a>
      <a href="#team" class="block py-3 hover:text-gold transition">Team</a>
      <a href="https://discord.gg/pGM8hT8tS6" target="_blank" class="block py-3 text-gold font-medium">Discord</a>
    </div>
  </header>

  <!-- HERO -->
  <section id="hero" class="min-h-screen flex flex-col justify-center items-center text-center px-6 pt-16">
    <div class="max-w-4xl mx-auto">
      <h1 class="text-6xl md:text-8xl font-black mb-6 tracking-tight fade-in">
        <span class="gold-gradient">MEGA</span>
        <span class="block text-4xl md:text-6xl mt-2">CITY RP</span>
      </h1>
      <p class="max-w-2xl mx-auto text-gray-300 text-xl mb-10 fade-in leading-relaxed">
        Tauche ein in eine lebendige Stadt voller Geschichten, Emotionen und realistischem RP.  
        Dein Abenteuer beginnt hier — fair, clean & immersiv.
      </p>
      <div class="flex flex-wrap justify-center gap-5 fade-in">
        <a href="regeln.html" class="px-8 py-3.5 bg-gold text-black font-bold rounded-lg hover:bg-yellow-400 transition shadow-lg transform hover:scale-105">Regelwerk</a>
        <a href="https://discord.gg/pGM8hT8tS6" target="_blank" class="px-8 py-3.5 border-2 border-gold/50 text-gold font-bold rounded-lg hover:bg-gold/10 transition transform hover:scale-105">Discord</a>
      </div>
    </div>
  </section>

  <!-- FEATURES -->
  <section id="features" class="py-24 px-6 border-t border-gray-800/50 fade-in">
    <div class="max-w-7xl mx-auto text-center">
      <h2 class="text-4xl font-bold mb-16 section-title gold-gradient">Was macht uns besonders?</h2>
      <div class="grid md:grid-cols-3 gap-8">
        <div class="card p-8 rounded-xl">
          <div class="w-14 h-14 bg-gold/10 rounded-lg flex items-center justify-center mb-5 mx-auto">
            <span class="text-2xl">🎭</span>
          </div>
          <h3 class="text-xl font-bold mb-3 text-gold">Realismus</h3>
          <p class="text-gray-400 leading-relaxed">Alle Interaktionen basieren auf glaubwürdigem Verhalten — kein Power- oder Fail-RP. Lebe deinen Charakter in einer konsistenten Welt.</p>
        </div>
        <div class="card p-8 rounded-xl">
          <div class="w-14 h-14 bg-gold/10 rounded-lg flex items-center justify-center mb-5 mx-auto">
            <span class="text-2xl">👥</span>
          </div>
          <h3 class="text-xl font-bold mb-3 text-gold">Community</h3>
          <p class="text-gray-400 leading-relaxed">Ein respektvolles, erwachsenes Umfeld mit Fokus auf Qualität statt Quantität. Gemeinsam erschaffen wir großartige Geschichten.</p>
        </div>
        <div class="card p-8 rounded-xl">
          <div class="w-14 h-14 bg-gold/10 rounded-lg flex items-center justify-center mb-5 mx-auto">
            <span class="text-2xl">⚡</span>
          </div>
          <h3 class="text-xl font-bold mb-3 text-gold">Performance</h3>
          <p class="text-gray-400 leading-relaxed">Optimierte Scripts, stabile Server und konstante Weiterentwicklung für flüssiges RP ohne technische Probleme.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- ABOUT -->
  <section id="about" class="py-24 px-6 border-t border-gray-800/50 fade-in">
    <div class="max-w-5xl mx-auto text-center">
      <h2 class="text-4xl font-bold mb-6 section-title gold-gradient">Über uns</h2>
      <p class="text-gray-300 text-lg leading-relaxed max-w-3xl mx-auto">
        Mega City RP ist ein moderner GTA V Roleplay-Server, der Realismus und Freiheit perfekt kombiniert.  
        Unsere Philosophie: faire Regeln, erwachsene Spieler und eine Stadt, die niemals schläft. 
        Wir setzen auf Qualitäts-RP, tiefgreifende Charakterentwicklung und eine lebendige Wirtschaft.
      </p>
    </div>
  </section>

  <!-- RULES (Short) -->
  <section id="rules" class="py-24 px-6 border-t border-gray-800/50 fade-in">
    <div class="max-w-7xl mx-auto">
      <h2 class="text-4xl font-bold mb-16 section-title gold-gradient text-center">Regelwerk (Kurzfassung)</h2>
      <div class="grid md:grid-cols-2 gap-10">
        <div class="card p-8 rounded-xl">
          <h3 class="text-2xl font-bold mb-6 text-gold text-center">Schnell-Infos</h3>
          <ul class="space-y-4 text-gray-300">
            <li class="flex items-start">
              <span class="text-gold mr-3">•</span>
              <span><strong>Sprache:</strong> Deutsch</span>
            </li>
            <li class="flex items-start">
              <span class="text-gold mr-3">•</span>
              <span><strong>Mindestalter:</strong> 18+</span>
            </li>
            <li class="flex items-start">
              <span class="text-gold mr-3">•</span>
              <span><strong>NLR:</strong> 30 Minuten</span>
            </li>
            <li class="flex items-start">
              <span class="text-gold mr-3">•</span>
              <span><strong>Max. Crime-Teamgröße:</strong> 4</span>
            </li>
            <li class="flex items-start">
              <span class="text-gold mr-3">•</span>
              <span><strong>Mic-Pflicht:</strong> Ja</span>
            </li>
          </ul>
        </div>
        <div class="card p-8 rounded-xl">
          <h3 class="text-2xl font-bold mb-6 text-gold text-center">Wichtigste Regeln</h3>
          <div class="space-y-5 text-gray-300">
            <p><strong class="text-gold">Respekt & Realismus:</strong> Sei fair, glaubwürdig und respektvoll. Keine Beleidigungen, kein Power-/Fail-RP.</p>
            <p><strong class="text-gold">RP-Grundlagen:</strong> NLR gilt 30 Minuten. Kein RDM, kein VDM. Jede Aktion braucht RP-Grundlage.</p>
            <p><strong class="text-gold">Technik & Kommunikation:</strong> Mic-Pflicht, keine Makros, keine Exploits. Supportfälle nur mit Videobeweis.</p>
            <div class="mt-6 pt-5 border-t border-gray-800">
              <p class="text-gold/80 italic text-sm">Für das vollständige Regelwerk klicke auf den Button unten.</p>
              <div class="mt-4">
                <a href="regeln.html" class="inline-block px-6 py-3 bg-gold text-black font-semibold rounded-lg hover:bg-yellow-400 transition shadow-md">Zum vollständigen Regelwerk</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- TEAM -->
  <section id="team" class="py-24 px-6 border-t border-gray-800/50 fade-in">
    <div class="max-w-7xl mx-auto text-center">
      <h2 class="text-4xl font-bold mb-16 section-title gold-gradient">Team & Kontakt</h2>
      <div class="grid md:grid-cols-3 gap-8">
        <div class="card p-8 rounded-xl">
          <div class="w-16 h-16 bg-gold/10 rounded-full flex items-center justify-center mb-5 mx-auto">
            <span class="text-2xl">👑</span>
          </div>
          <h3 class="text-xl font-bold mb-3 text-gold">Leitung</h3>
          <p class="text-gray-400">Verantwortlich für Serverkonzept und -entwicklung</p>
          <p class="text-gold mt-3 text-sm">Kontakt über Discord</p>
        </div>
        <div class="card p-8 rounded-xl">
          <div class="w-16 h-16 bg-gold/10 rounded-full flex items-center justify-center mb-5 mx-auto">
            <span class="text-2xl">🛠️</span>
          </div>
          <h3 class="text-xl font-bold mb-3 text-gold">Support</h3>
          <p class="text-gray-400">Hilfe bei Fragen und Regelverstößen</p>
          <p class="text-gold mt-3 text-sm">Ticket-System im Discord</p>
        </div>
        <div class="card p-8 rounded-xl">
          <div class="w-16 h-16 bg-gold/10 rounded-full flex items-center justify-center mb-5 mx-auto">
            <span class="text-2xl">⚙️</span>
          </div>
          <h3 class="text-xl font-bold mb-3 text-gold">Technik</h3>
          <p class="text-gray-400">Serverwartung und Scripting</p>
          <p class="text-gold mt-3 text-sm">Server-IP: <span class="font-mono">mega.city</span></p>
        </div>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer class="border-t border-gray-800 py-12 text-center text-gray-500 bg-black/70">
    <div class="max-w-7xl mx-auto px-6">
      <div class="flex flex-col md:flex-row justify-between items-center gap-6 mb-8">
        <div class="flex items-center gap-3">
          <img src="mlogo42.png" alt="Mega City RP Logo" class="h-10 w-10 rounded-md object-cover ring-1 ring-gold/30" />
          <div class="text-left">
            <div class="font-bold text-white">Mega City RP</div>
            <div class="text-xs text-gray-400">Clean · Realistisch · Fair</div>
          </div>
        </div>
        <div class="flex gap-6">
          <a href="#features" class="text-gray-400 hover:text-gold transition">Features</a>
          <a href="regeln.html" class="text-gray-400 hover:text-gold transition">Regeln</a>
          <a href="#about" class="text-gray-400 hover:text-gold transition">Über uns</a>
          <a href="#team" class="text-gray-400 hover:text-gold transition">Team</a>
        </div>
        <a href="https://discord.gg/pGM8hT8tS6" target="_blank" class="px-5 py-2.5 bg-gold text-black font-semibold rounded-lg hover:bg-yellow-400 transition text-sm">Discord</a>
      </div>
      <p class="pt-6 border-t border-gray-800/50">© <span id="year"></span> Mega City RP • Alle Rechte vorbehalten</p>
    </div>
  </footer>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
    document.getElementById('mobileBtn').addEventListener('click', () => {
      document.getElementById('mobileMenu').classList.toggle('hidden');
    });
    
    // Scroll fade-in
    const observer = new IntersectionObserver(entries => {
      entries.forEach(e => {
        if (e.isIntersecting) e.target.classList.add('visible');
      });
    }, { threshold: 0.1 });
    document.querySelectorAll('.fade-in').forEach(el => observer.observe(el));
    
    // Navbar animation on scroll
    const navbar = document.getElementById('navbar');
    let lastScrollY = 0;
    window.addEventListener('scroll', () => {
      if (window.scrollY > 50) {
        navbar.classList.add('bg-black/90', 'shadow-lg');
        navbar.classList.remove('glass');
      } else {
        navbar.classList.remove('bg-black/90', 'shadow-lg');
        navbar.classList.add('glass');
      }

      // Hide when scrolling down, show when scrolling up
      if (window.scrollY > lastScrollY && window.scrollY > 200) {
        navbar.style.transform = 'translateY(-100%)';
      } else {
        navbar.style.transform = 'translateY(0)';
      }
      lastScrollY = window.scrollY;
    });
  </script>
</body>
</html>
