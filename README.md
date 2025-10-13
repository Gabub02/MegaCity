<!--
  Mega City RP - OnePage
  - Tailwind CSS (CDN) used (no build step required)
  - Replace DISCORD_INVITE_HERE with your real Discord invite URL
  - Add logo by replacing the <img> src in the header
  - Save this file as index.html and upload to any static host (Netlify, GitHub Pages, Vercel, etc.)
-->

<!doctype html>
<html lang="de">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Mega City RP — Regelwerk & Info</title>
  <meta name="description" content="Mega City RP — Clean, realistisches GTA V Roleplay. Regelwerk, Team & Kontakt." />
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    // Tailwind custom colors
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
    /* Small extra polishing */
    .glass { background: rgba(255,255,255,0.04); backdrop-filter: blur(6px); }
    .card { background: rgba(255,255,255,0.03); }
    .rule-scroll { max-height: 60vh; overflow:auto; scroll-behavior:smooth; }
  </style>
</head>
<body class="bg-gradient-to-b from-mcblack via-gray-900 to-black text-gray-100 antialiased leading-relaxed">
  <header class="sticky top-0 z-50">
    <nav class="max-w-6xl mx-auto px-6 py-4 flex items-center justify-between">
      <div class="flex items-center gap-4">
        <!-- Replace the src with your logo path -->
        <img src="mlogo42.png" alt="Mega City RP Logo" class="h-12 w-12 rounded-md bg-white/5 object-cover" />
        <div>
          <a href="#hero" class="text-xl font-semibold tracking-tight">Mega City RP</a>
          <div class="text-xs text-gray-400 -mt-0.5">Clean · Realistisch · Fair</div>
        </div>
      </div>
      <div class="hidden md:flex gap-6 items-center">
        <a href="#rules" class="hover:text-gold">Regeln</a>
        <a href="#about" class="hover:text-gold">Über uns</a>
        <a href="#team" class="hover:text-gold">Team</a>
        <a href="https://discord.gg/nwmmTfnz" target="_blank" class="inline-flex items-center gap-2 bg-gold/10 text-gold px-4 py-2 rounded-lg border border-gold/20 hover:bg-gold/20">Discord</a>
      </div>
      <div class="md:hidden">
        <button id="mobileBtn" class="p-2 rounded-md glass">☰</button>
      </div>
    </nav>
    <div id="mobileMenu" class="hidden bg-gray-900/60 glass px-6 py-4 md:hidden">
      <a href="#rules" class="block py-2">Regeln</a>
      <a href="#about" class="block py-2">Über uns</a>
      <a href="#team" class="block py-2">Team</a>
      <a href="DISCORD_INVITE_HERE" target="_blank" class="block py-2">Discord</a>
    </div>
  </header>

  <main class="max-w-6xl mx-auto px-6 py-12">
    <!-- HERO -->
    <section id="hero" class="flex flex-col md:flex-row items-center gap-8 py-12">
      <div class="flex-1">
        <h1 class="text-4xl md:text-6xl font-extrabold tracking-tight">Mega City RP</h1>
        <p class="mt-4 text-lg text-gray-300 max-w-2xl">Cleanes, realistisches GTA V Roleplay – fair moderiert, mit Fokus auf Immersion und guter Community. Lies das Regelwerk, bevor du spielst.</p>
        <div class="mt-6 flex gap-3">
          <a href="#rules" class="px-6 py-3 bg-gold text-black rounded-lg font-semibold shadow">Regelwerk lesen</a>
          <a href="DISCORD_INVITE_HERE" target="_blank" class="px-6 py-3 border border-gold/30 rounded-lg">Discord beitreten</a>
        </div>
      </div>
      <div class="flex-1">
        <div class="h-60 md:h-48 rounded-xl overflow-hidden bg-gradient-to-br from-gray-800 to-black card p-6 flex items-end">
          <div>
            <div class="text-sm text-gray-400">Server-Info</div>
            <div class="text-xl font-semibold">IP: <span class="text-gold">mega.city</span></div>
            <div class="text-sm text-gray-400">Whitelist: Optional · Mindestalter: 18+</div>
          </div>
        </div>
      </div>
    </section>

    <!-- ABOUT -->
    <section id="about" class="py-8 border-t border-gray-800">
      <h2 class="text-2xl font-bold">Über Mega City RP</h2>
      <p class="mt-3 text-gray-300 max-w-3xl">Mega City RP ist ein moderner, sauber moderierter GTA V Roleplay-Server. Unser Fokus liegt auf realistischem Roleplay, respektvollem Miteinander und einer Community, die zusammen spannende Geschichten schreibt. Fairness, Performance und klare Regeln sind unsere Priorität.</p>
    </section>

    <!-- RULES -->
    <section id="rules" class="py-8 border-t border-gray-800">
      <h2 class="text-2xl font-bold">Regelwerk</h2>
      <div class="mt-4 grid grid-cols-1 md:grid-cols-3 gap-6">
        <aside class="md:col-span-1">
          <div class="p-4 rounded-lg card">
            <h3 class="font-semibold">Schnell-Infos</h3>
            <ul class="mt-3 text-sm text-gray-300 space-y-2">
              <li>Sprache: Deutsch</li>
              <li>Mindestalter: 18+</li>
              <li>NLR (New-Life-Regel): 30 Minuten</li>
              <li>Max. Gruppengröße (Crime): 4</li>
            </ul>
          </div>
        </aside>

        <div class="md:col-span-2">
          <div class="p-6 rounded-lg card rule-scroll">
            <!-- Inserted cleaned rule content below -->

            <h4 class="text-lg font-semibold">Willkommen</h4>
            <p class="mt-2 text-gray-300">Mit dem Betreten des Servers akzeptierst du automatisch alle Regeln. Mega City RP steht für realistisches, faires und immersives Roleplay. Behandle andere Spieler respektvoll und spiele glaubwürdig.</p>

            <h4 class="mt-4 font-semibold">Allgemeine Regeln</h4>
            <ol class="list-decimal list-inside mt-2 text-gray-300 space-y-2">
              <li>Die Regeln müssen bekannt und eingehalten werden. Unwissenheit schützt nicht.</li>
              <li>Respektvolles Verhalten ist Pflicht. Diskriminierung, Mobbing, Rassismus oder sexistische Inhalte sind verboten.</li>
              <li>Cheats, Mod-Menüs, Exploits, Bug-Using und Makros sind verboten und führen zu permanentem Bann.</li>
              <li>Wer Bugs findet, meldet diese sofort im Support. Das Ausnutzen ist untersagt.</li>
              <li>Werbung für andere Communities ist verboten.</li>
            </ol>

            <h4 class="mt-4 font-semibold">Roleplay-Grundsätze</h4>
            <ul class="mt-2 text-gray-300 space-y-2">
              <li><strong>In-Character (IC)</strong> vor Out-of-Character (OOC). OOC nur, wenn nötig (z. B. Supportfälle).</li>
              <li><strong>Power-RP</strong> & <strong>Fail-RP</strong> sind verboten: Keine erzwungenen Aktionen ohne Reaktionsmöglichkeit; keine unrealistischen Handlungen.</li>
              <li><strong>Fear-RP:</strong> Spiele Angst und Vorsicht in gefährlichen Situationen; handle so, dass das Leben deines Charakters Gewicht hat.</li>
              <li>New-Life-Regel (NLR): Nach dem Tod 30 Minuten nicht zurückkehren oder Wissen verwenden, das aus der Situation stammt.</li>
              <li>Charaktere sollen realistisch gestaltet und gespielt werden.</li>
            </ul>

            <h4 class="mt-4 font-semibold">Crime & Polizei</h4>
            <ul class="mt-2 text-gray-300 space-y-2">
              <li>Kriminelle Aktionen müssen RP-begründet sein. Zufälliges Ausrauben zur reinen Bereicherung ist verboten (Eigenbereicherung).</li>
              <li>RDM (Random Deathmatch) und VDM (Vehicle Deathmatch) sind untersagt.</li>
              <li>Geiselnahmen, Bank- und Spezialraub müssen mit angemessener RP-Basis stattfinden (Geiseln, Verhandlungen etc.).</li>
              <li>Nach Schießereien gilt NLR: 30 Minuten kein erneutes Betreten der Situation.</li>
              <li>Maximale Standard-Größe von kriminellen Aktionen: 4 Personen (sofern nicht anders erlaubt).</li>
            </ul>

            <h4 class="mt-4 font-semibold">Fahrzeug- & Verkehrsregeln</h4>
            <ul class="mt-2 text-gray-300 space-y-2">
              <li>Fahrzeuge realistisch fahren – keine Stunts in der Innenstadt; respektvolles Fahren in belebten Zonen.</li>
              <li>Verfolgungen und Drive-Bys nur mit nachvollziehbarem RP-Hintergrund; Schüsse aus Fahrzeugen auf Fußgänger sind erlaubt, zwischen Fahrzeugen hingegen nur in seltenen, ausgespielten Fällen.</li>
              <li>Fahrzeuge dürfen nur mit realistischem RP-Hintergrund gestohlen werden. Dienstfahrzeuge der Staatsfraktionen sind geschützt.</li>
            </ul>

            <h4 class="mt-4 font-semibold">Kommunikation & Technik</h4>
            <ul class="mt-2 text-gray-300 space-y-2">
              <li>Kein Meta-Gaming: Infos aus Streams, Discord oder OOC dürfen nicht IC genutzt werden.</li>
              <li>Kein Stream-Sniping. Keine Zusammenarbeit mit Zuschauern zur Einflussnahme auf RP.</li>
              <li>Mikrofonpflicht in RP-Situationen; schlechte Mikrofonqualität oder Stimmverzerrer sind nicht erlaubt.</li>
            </ul>

            <h4 class="mt-4 font-semibold">Support & Beweise</h4>
            <ul class="mt-2 text-gray-300 space-y-2">
              <li>Regelverstöße melden mit Videobeweis (komplette Situation inkl. Ton). Supportfälle innerhalb von 48 Stunden melden.</li>
              <li>Supportgespräche sind vertraulich und dürfen nicht veröffentlicht werden.</li>
              <li>Der leitende Supporter entscheidet über den Fall; Widerspruch ist per Ticket möglich.</li>
            </ul>

            <h4 class="mt-4 font-semibold">Spezielle Regeln (Kurz)</h4>
            <ul class="mt-2 text-gray-300 space-y-2">
              <li>Mindestalter Server/Char: 18+</li>
              <li>Unantastbarkeiten (z. B. Medics, Mechaniker, Anwälte u.ä.) gelten, solange sie nicht selbst angreifen.</li>
              <li>Verstecken von mehreren Personen im Kofferraum gilt als Bug-Using und ist verboten.</li>
              <li>Geiseln verhungern/verdursten lassen ist verboten; humane Behandlung ist Pflicht.</li>
              <li>Tierrechte: Gewalt gegen Tiere führt zum permanenten Bann.</li>
            </ul>

            <h4 class="mt-4 font-semibold">Blacklist & OOC-Ausdrücke</h4>
            <p class="text-gray-300">Das Verwenden von bestimmten beleidigenden, rassistischen oder den Support betreffenden Schimpfwörtern ist verboten. (Detaillierte Blacklist wird im Discord geführt.)</p>

            <h4 class="mt-4 font-semibold">Änderungen & Abschluss</h4>
            <p class="text-gray-300">Das Team behält sich Änderungen des Regelwerks vor. Änderungen werden im Kanal <code>#regelwerk-änderungen</code> auf Discord veröffentlicht. Bei Fragen: Support öffnen.</p>

            <!-- End of rule content -->
          </div>
        </div>
      </div>
    </section>

    <!-- TEAM / CONTACT -->
    <section id="team" class="py-8 border-t border-gray-800">
      <h2 class="text-2xl font-bold">Team & Kontakt</h2>
      <p class="mt-3 text-gray-300 max-w-3xl">Unser Team besteht aus erfahrenen Supportern & Moderatoren, die für ein faires und sicheres Spielerlebnis sorgen. Kontaktiere uns über Discord für Support oder Fragen.</p>
      <div class="mt-6 grid grid-cols-1 md:grid-cols-3 gap-4">
        <div class="p-4 rounded-lg card">
          <div class="font-semibold">Lead Admin</div>
          <div class="text-sm text-gray-400">Kontakt über Discord</div>
        </div>
        <div class="p-4 rounded-lg card">
          <div class="font-semibold">Support & Moderation</div>
          <div class="text-sm text-gray-400">Ticket-System im Discord</div>
        </div>
        <div class="p-4 rounded-lg card">
          <div class="font-semibold">Technik & Server</div>
          <div class="text-sm text-gray-400">Serverstatus & IP: mega.city (Platzhalter)</div>
        </div>
      </div>
    </section>

    <!-- FOOTER -->
    <footer class="mt-12 border-t border-gray-800 pt-8 pb-12 text-center text-gray-400">
      <div class="max-w-3xl mx-auto">© <span id="year"></span> Mega City RP — All rights reserved. • <a href=https://discord.gg/nwmmTfnz class="hover:text-gold">Discord</a></div>
    </footer>
  </main>

  <script>
    // small scripts
    document.getElementById('year').innerText = new Date().getFullYear();
    const btn = document.getElementById('mobileBtn');
    const menu = document.getElementById('mobileMenu');
    btn?.addEventListener('click', ()=>{ menu.classList.toggle('hidden') });
  </script>
</body>
</html>
