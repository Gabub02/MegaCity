<!-- FILE: index.html -->
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
    html { scroll-behavior: smooth; }
    body { overflow-x: hidden; }
    .glass { background: rgba(255,255,255,0.05); backdrop-filter: blur(8px); }
    .card { background: rgba(255,255,255,0.03); transition: all 0.3s ease; }
    .card:hover { background: rgba(255,255,255,0.07); transform: translateY(-4px); }
    .glow { text-shadow: 0 0 18px rgba(255,215,0,0.35); }
    .fade-in { opacity: 0; transform: translateY(20px); transition: all 0.8s ease-out; }
    .fade-in.visible { opacity: 1; transform: translateY(0); }
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
  </style>
</head>
<body class="bg-gradient-to-b from-black via-gray-900 to-mcblack text-gray-100 antialiased relative">

  <div class="bg-animate"></div>

  <!-- HEADER -->
<header id="navbar" class="fixed w-full z-50 bg-black/70 backdrop-blur-md border-b border-gray-800 transition-all duration-500">
  <nav class="max-w-6xl mx-auto px-6 py-4 flex items-center justify-between">
    <div class="flex items-center gap-3">
      <img src="mlogo42.png" alt="Mega City RP Logo" class="h-10 w-10 rounded-md object-cover ring-1 ring-gold/30" />
      <div>
        <a href="#hero" class="text-lg font-semibold glow">Mega City RP</a>
        <p class="text-xs text-gray-400 -mt-0.5">Clean · Realistisch · Fair</p>
      </div>
    </div>
    <div class="hidden md:flex gap-8 items-center text-sm">
      <a href="#features" class="hover:text-gold transition">Features</a>
      <a href="regeln.html" class="hover:text-gold transition">Regeln</a>
      <a href="#about" class="hover:text-gold transition">Über uns</a>
      <a href="#team" class="hover:text-gold transition">Team</a>
      <a href="https://discord.gg/pGM8hT8tS6" target="_blank" class="px-4 py-2 border border-gold/40 text-gold rounded-lg hover:bg-gold hover:text-black transition">Discord</a>
    </div>
    <button id="mobileBtn" class="md:hidden p-2 text-xl">☰</button>
  </nav>
  <div id="mobileMenu" class="hidden md:hidden bg-black/90 text-center py-3">
    <a href="#features" class="block py-2 hover:text-gold">Features</a>
    <a href="regeln.html" class="block py-2 hover:text-gold">Regeln</a>
    <a href="#about" class="block py-2 hover:text-gold">Über uns</a>
    <a href="#team" class="block py-2 hover:text-gold">Team</a>
    <a href="https://discord.gg/pGM8hT8tS6" target="_blank" class="block py-2 text-gold">Discord</a>
  </div>
</header>

  <!-- HERO -->
  <section id="hero" class="min-h-screen flex flex-col justify-center items-center text-center px-6">
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
            <a href="regeln.html" class="px-4 py-2 bg-gold text-black rounded-lg font-semibold">Zum vollständigen Regelwerk</a>
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
    <p>© <span id="year"></span> Mega City RP • Alle Rechte vorbehalten • <a href="DISCORD_INVITE_HERE" class="hover:text-gold">Discord</a></p>
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
    }, { threshold: 0.12 });
    document.querySelectorAll('.fade-in').forEach(el => observer.observe(el));
  </script>
</body>
</html>



<!-- FILE: regeln.html -->
<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Mega City RP — Vollständiges Regelwerk</title>
  <meta name="description" content="Mega City RP — Vollständiges Regelwerk und Informationen." />
  <meta name="theme-color" content="#FFD700" />
  <link rel="icon" href="mlogo42.png" type="image/png" />
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            gold: '#FFD700',
            mcblack: '#0b0b0b'
          }
        }
      }
    }
  </script>
  <style>
    html { scroll-behavior: smooth; }
    body { background: linear-gradient(180deg, #000000 0%, #070707 100%); color: #e6e6e6; }
    .container { max-width: 900px; margin: 0 auto; padding: 36px; }
    .card { background: rgba(255,255,255,0.02); padding: 24px; border-radius: 12px; box-shadow: 0 6px 30px rgba(0,0,0,0.6); }
    .rule-title { color: #FFD700; text-shadow: 0 0 8px rgba(255,215,0,0.12); }
    pre { white-space: pre-wrap; }
  </style>
</head>
<body>
  <header class="bg-black/80 backdrop-blur-md border-b border-gray-800 fixed w-full z-50">
    <nav class="max-w-6xl mx-auto px-6 py-4 flex items-center justify-between">
      <div class="flex items-center gap-3">
        <a href="index.html" class="text-lg font-semibold text-gold">← Zurück</a>
      </div>
      <div class="text-sm text-gray-400">Mega City RP — Vollständiges Regelwerk</div>
    </nav>
  </header>

  <main class="container" style="padding-top:110px;">
    <div class="card">
      <h1 class="text-2xl font-bold rule-title">Regelwerk — Mega City RP</h1>
      <p class="mt-2 text-gray-300">Mit dem Betreten des Servers akzeptierst du automatisch alle Regeln. Mega City RP steht für realistisches, faires und immersives Roleplay. Behandle andere Spieler respektvoll und spiele glaubwürdig.</p>

      <h2 class="mt-6 font-semibold">Allgemeine Regeln</h2>
      <ol class="list-decimal list-inside mt-2 text-gray-300 space-y-2">
        <li>Die Regeln müssen bekannt und eingehalten werden. Unwissenheit schützt nicht.</li>
        <li>Respektvolles Verhalten ist Pflicht. Diskriminierung, Mobbing, Rassismus oder sexistische Inhalte sind verboten.</li>
        <li>Cheats, Mod-Menüs, Exploits, Bug-Using und Makros sind verboten und führen zu permanentem Bann.</li>
        <li>Wer Bugs findet, meldet diese sofort im Support. Das Ausnutzen ist untersagt.</li>
        <li>Werbung für andere Communities ist verboten.</li>
      </ol>

      <h2 class="mt-6 font-semibold">Roleplay-Grundsätze</h2>
      <ul class="mt-2 text-gray-300 space-y-2">
        <li><strong>In-Character (IC)</strong> vor Out-of-Character (OOC). OOC nur, wenn nötig (z. B. Supportfälle).</li>
        <li><strong>Power-RP</strong> & <strong>Fail-RP</strong> sind verboten: Keine erzwungenen Aktionen ohne Reaktionsmöglichkeit; keine unrealistischen Handlungen.</li>
        <li><strong>Fear-RP:</strong> Spiele Angst und Vorsicht in gefährlichen Situationen; handle so, dass das Leben deines Charakters Gewicht hat.</li>
        <li>New-Life-Regel (NLR): Nach dem Tod 30 Minuten nicht zurückkehren oder Wissen verwenden, das aus der Situation stammt.</li>
        <li>Charaktere sollen realistisch gestaltet und gespielt werden.</li>
      </ul>

      <h2 class="mt-6 font-semibold">Crime & Polizei</h2>
      <ul class="mt-2 text-gray-300 space-y-2">
        <li>Kriminelle Aktionen müssen RP-begründet sein. Zufälliges Ausrauben zur reinen Bereicherung ist verboten (Eigenbereicherung).</li>
        <li>RDM (Random Deathmatch) und VDM (Vehicle Deathmatch) sind untersagt.</li>
        <li>Geiselnahmen, Bank- und Spezialraub müssen mit angemessener RP-Basis stattfinden (Geiseln, Verhandlungen etc.).</li>
        <li>Nach Schießereien gilt NLR: 30 Minuten kein erneutes Betreten der Situation.</li>
        <li>Maximale Standard-Größe von kriminellen Aktionen: 4 Personen (sofern nicht anders erlaubt).</li>
      </ul>

      <h2 class="mt-6 font-semibold">Fahrzeug- & Verkehrsregeln</h2>
      <ul class="mt-2 text-gray-300 space-y-2">
        <li>Fahrzeuge realistisch fahren – keine Stunts in der Innenstadt; respektvolles Fahren in belebten Zonen.</li>
        <li>Verfolgungen und Drive-Bys nur mit nachvollziehbarem RP-Hintergrund; Schüsse aus Fahrzeugen auf Fußgänger sind erlaubt, zwischen Fahrzeugen hingegen nur in seltenen, ausgespielten Fällen.</li>
        <li>Fahrzeuge dürfen nur mit realistischem RP-Hintergrund gestohlen werden. Dienstfahrzeuge der Staatsfraktionen sind geschützt.</li>
      </ul>

      <h2 class="mt-6 font-semibold">Kommunikation & Technik</h2>
      <ul class="mt-2 text-gray-300 space-y-2">
        <li>Kein Meta-Gaming: Infos aus Streams, Discord oder OOC dürfen nicht IC genutzt werden.</li>
        <li>Kein Stream-Sniping. Keine Zusammenarbeit mit Zuschauern zur Einflussnahme auf RP.</li>
        <li>Mikrofonpflicht in RP-Situationen; schlechte Mikrofonqualität oder Stimmverzerrer sind nicht erlaubt.</li>
      </ul>

      <h2 class="mt-6 font-semibold">Support & Beweise</h2>
      <ul class="mt-2 text-gray-300 space-y-2">
        <li>Regelverstöße melden mit Videobeweis (komplette Situation inkl. Ton). Supportfälle innerhalb von 48 Stunden melden.</li>
        <li>Supportgespräche sind vertraulich und dürfen nicht veröffentlicht werden.</li>
        <li>Der leitende Supporter entscheidet über den Fall; Widerspruch ist per Ticket möglich.</li>
      </ul>

      <h2 class="mt-6 font-semibold">Spezielle Regeln (Kurz)</h2>
      <ul class="mt-2 text-gray-300 space-y-2">
        <li>Mindestalter Server/Char: 18+</li>
        <li>Unantastbarkeiten (z. B. Medics, Mechaniker, Anwälte u.ä.) gelten, solange sie nicht selbst angreifen.</li>
        <li>Verstecken von mehreren Personen im Kofferraum gilt als Bug-Using und ist verboten.</li>
        <li>Geiseln verhungern/verdursten lassen ist verboten; humane Behandlung ist Pflicht.</li>
        <li>Tierrechte: Gewalt gegen Tiere führt zum permanenten Bann.</li>
      </ul>

      <h2 class="mt-6 font-semibold">Blacklist & OOC-Ausdrücke</h2>
      <p class="text-gray-300">Das Verwenden von bestimmten beleidigenden, rassistischen oder den Support betreffenden Schimpfwörtern ist verboten. (Detaillierte Blacklist wird im Discord geführt.)</p>

      <h2 class="mt-6 font-semibold">Änderungen & Abschluss</h2>
      <p class="text-gray-300">Das Team behält sich Änderungen des Regelwerks vor. Änderungen werden im Kanal <code>#regelwerk-änderungen</code> auf Discord veröffentlicht. Bei Fragen: Support öffnen.</p>

      <hr class="my-6 border-gray-700" />
      <p class="text-sm text-gray-400">Stand: <span id="ruleDate"></span></p>
    </div>
  </main>

  <footer style="position:fixed;left:0;right:0;bottom:0;padding:12px;background:rgba(0,0,0,0.6);text-align:center;color:#c9c9c9;">© <span id="yearFooter"></span> Mega City RP</footer>

  <script>
    // set dates and small UI
    document.getElementById('ruleDate').innerText = new Date().toLocaleDateString('de-DE');
    document.getElementById('yearFooter').innerText = new Date().getFullYear();
  </script>
</body>
</html>
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
    }, { threshold: 0.12 });
    document.querySelectorAll('.fade-in').forEach(el => observer.observe(el));

    // Navbar animation on scroll
    const navbar = document.getElementById('navbar');
    let lastScrollY = 0;
    window.addEventListener('scroll', () => {
      if (window.scrollY > 50) {
        navbar.classList.add('bg-black/90', 'shadow-lg');
        navbar.classList.remove('bg-black/70');
      } else {
        navbar.classList.remove('bg-black/90', 'shadow-lg');
        navbar.classList.add('bg-black/70');
      }

      // Optional: hide when scrolling down, show when scrolling up
      if (window.scrollY > lastScrollY && window.scrollY > 200) {
        navbar.style.transform = 'translateY(-100%)';
      } else {
        navbar.style.transform = 'translateY(0)';
      }
      lastScrollY = window.scrollY;
    });
  </script>

