

<!doctype html><html><head><meta charset=utf8><meta name=viewport content="width=device-width,initial-scale=1,viewport-fit=cover"><style>:root{color-scheme:light;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}html{scroll-padding-top:env(safe-area-inset-top,0px)}body{margin:0;padding:0;font:14px -apple-system,BlinkMacSystemFont,sans-serif;background:#fff;color:#000}img{max-width:100%}[hidden]:not([hidden=until-found i]){display:none!important}</style></head><body>
<title>Ibrahima Ben Mady Kebe</title>
<meta name="claude:viewport-fit-sides" content="cover">
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:wght@500;700;800&family=IBM+Plex+Sans:wght@400;500;600&family=IBM+Plex+Mono:wght@400;500&display=swap">
<style>
/* Concept : une page à deux couleurs. Le bleu marque tout ce qui relève des TI, l'ambre tout ce qui relève de la gestion.
   Les éléments qui touchent aux deux prennent les deux teintes. */
:root {
  --bg: #F3F6F8;
  --surface: #FFFFFF;
  --ink: #0D2231;
  --ink-2: #4A5F6E;
  --line: #D3DDE4;
  --ti: #1A5276;
  --ti-soft: #DCEAF3;
  --ge: #8A5200;
  --ge-fill: #E9A23B;
  --ge-soft: #F8E9CF;
  --focus: #1A5276;
  --font-display: 'Bricolage Grotesque', 'Arial Narrow', Arial, sans-serif;
  --font-body: 'IBM Plex Sans', system-ui, -apple-system, 'Segoe UI', sans-serif;
  --font-mono: 'IBM Plex Mono', ui-monospace, 'SFMono-Regular', Menlo, monospace;
}
@media (prefers-color-scheme: dark) {
  :root:not([data-theme="light"]) {
    --bg: #0A1621; --surface: #112232; --ink: #E7EEF3; --ink-2: #9FB2C0; --line: #223647;
    --ti: #6DB3E0; --ti-soft: #153A55; --ge: #F0B25A; --ge-fill: #F0B25A; --ge-soft: #3B2C14; --focus: #6DB3E0;
    color-scheme: dark;
  }
}
:root[data-theme="dark"] {
  --bg: #0A1621; --surface: #112232; --ink: #E7EEF3; --ink-2: #9FB2C0; --line: #223647;
  --ti: #6DB3E0; --ti-soft: #153A55; --ge: #F0B25A; --ge-fill: #F0B25A; --ge-soft: #3B2C14; --focus: #6DB3E0;
  color-scheme: dark;
}

*, *::before, *::after { box-sizing: border-box; }
html { scroll-behavior: smooth; scroll-padding-top: 76px; }
body {
  background: var(--bg); color: var(--ink);
  font-family: var(--font-body); font-size: 17px; line-height: 1.6;
  -webkit-font-smoothing: antialiased;
}
body::before { content: ""; position: fixed; inset: 0 0 auto; height: env(safe-area-inset-top, 0px); z-index: 30; background: var(--bg); }
a { color: inherit; }
:focus-visible { outline: 3px solid var(--focus); outline-offset: 3px; border-radius: 4px; }
h1, h2, h3 { font-family: var(--font-display); line-height: 1.08; text-wrap: balance; margin: 0; letter-spacing: -0.02em; }
p { margin: 0; }
ul { margin: 0; padding: 0; list-style: none; }

.wrap { max-width: 1120px; margin: 0 auto; padding-left: max(16px, env(safe-area-inset-left, 0px)); padding-right: max(16px, env(safe-area-inset-right, 0px)); }
.eyebrow { font-family: var(--font-mono); font-size: 12.5px; letter-spacing: .14em; text-transform: uppercase; color: var(--ink-2); }
.ti-text { color: var(--ti); }
.ge-text { color: var(--ge); }

/* En-tête */
.top { position: sticky; top: env(safe-area-inset-top, 0px); z-index: 20; background: var(--bg); border-bottom: 1px solid var(--line); }
.top .wrap { display: flex; align-items: center; justify-content: space-between; gap: 16px; padding-block: 12px; }
.brand { font-family: var(--font-display); font-weight: 800; font-size: 19px; text-decoration: none; letter-spacing: -0.01em; white-space: nowrap; }
.brand span:first-child { color: var(--ti); }
.brand span:last-child { color: var(--ge); }
.nav { display: flex; gap: 4px; overflow-x: auto; scrollbar-width: none; }
.nav::-webkit-scrollbar { display: none; }
.nav a { font-size: 14.5px; font-weight: 500; text-decoration: none; padding: 6px 10px; border-radius: 6px; color: var(--ink-2); white-space: nowrap; }
.nav a:hover { color: var(--ink); background: var(--surface); }

/* Héros */
.hero { padding-block: clamp(40px, 7vw, 88px) clamp(32px, 5vw, 56px); }
.hero .wrap { display: grid; grid-template-columns: minmax(0, 1.15fr) minmax(0, .85fr); gap: clamp(24px, 5vw, 64px); align-items: center; }
.hero h1 { font-size: clamp(2.5rem, 6.6vw, 4.9rem); font-weight: 800; margin-top: 18px; }
.hero .lede { margin-top: 24px; font-size: clamp(1.05rem, 1.6vw, 1.22rem); color: var(--ink-2); max-width: 36em; }
.actions { display: flex; flex-wrap: wrap; gap: 12px; margin-top: 32px; }
.btn { display: inline-flex; align-items: center; gap: 8px; font: 600 15.5px var(--font-body); padding: 12px 20px; border-radius: 8px; text-decoration: none; border: 1.5px solid var(--ink); color: var(--ink); background: transparent; cursor: pointer; }
.btn:hover { background: var(--surface); }
.btn.primary { background: var(--ink); color: var(--bg); }
.btn.primary:hover { background: var(--ti); border-color: var(--ti); color: #fff; }
.hero-art { width: 100%; max-width: 520px; justify-self: end; }
.hero-art svg { display: block; width: 100%; height: auto; }

.facts { margin-top: clamp(36px, 5vw, 64px); display: grid; grid-template-columns: repeat(4, minmax(0, 1fr)); border-top: 1px solid var(--line); }
.facts div { padding: 16px 16px 0 0; }
.facts dt { font-family: var(--font-mono); font-size: 12px; letter-spacing: .12em; text-transform: uppercase; color: var(--ink-2); }
.facts dd { margin: 6px 0 0; font-weight: 500; font-size: 15.5px; line-height: 1.4; }

/* Sections */
.section { padding-block: clamp(48px, 7vw, 96px); border-top: 1px solid var(--line); }
.section-head { display: grid; grid-template-columns: minmax(0, 5fr) minmax(0, 7fr); gap: clamp(16px, 4vw, 56px); align-items: end; margin-bottom: clamp(28px, 4vw, 48px); }
.section-head h2 { font-size: clamp(1.9rem, 4vw, 3rem); font-weight: 800; margin-top: 10px; }
.section-head p { color: var(--ink-2); max-width: 38em; }

/* Profil hybride */
.filters { display: flex; flex-wrap: wrap; gap: 8px; margin-bottom: 24px; }
.filter { font: 500 14.5px var(--font-body); padding: 8px 14px; border-radius: 8px; border: 1.5px solid var(--line); background: var(--surface); color: var(--ink); cursor: pointer; }
.filter:hover { border-color: var(--ink-2); }
.filter[aria-pressed="true"] { background: var(--ink); border-color: var(--ink); color: var(--bg); }
.bridge { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 16px; }
.col { background: var(--surface); border: 1px solid var(--line); border-radius: 10px; padding: 22px; transition: opacity .25s; }
.col[data-dim="true"] { opacity: .28; }
.col h3 { font-size: 1.35rem; font-weight: 700; }
.col .sub { margin-top: 4px; font-size: 14.5px; color: var(--ink-2); }
.col[data-kind="ti"] { border-top: 4px solid var(--ti); }
.col[data-kind="ge"] { border-top: 4px solid var(--ge-fill); }
.col[data-kind="both"] { border-top: 4px solid transparent; border-image: linear-gradient(90deg, var(--ti), var(--ge-fill)) 1; }
.chips { display: flex; flex-wrap: wrap; gap: 8px; margin-top: 18px; }
.chip { font-family: var(--font-mono); font-size: 13px; padding: 5px 9px; border-radius: 5px; border: 1px solid transparent; line-height: 1.3; }
.chip.ti { background: var(--ti-soft); color: var(--ti); border-color: color-mix(in srgb, var(--ti) 35%, transparent); }
.chip.ge { background: var(--ge-soft); color: var(--ge); border-color: color-mix(in srgb, var(--ge) 35%, transparent); }
.chip.both { background: linear-gradient(90deg, var(--ti-soft), var(--ge-soft)); color: var(--ink); border-color: var(--line); }
.formation { margin-top: 24px; display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 16px; }
.formation div { border-top: 1px solid var(--line); padding-top: 14px; }
.formation .eyebrow { display: block; }
.formation strong { display: block; margin-top: 4px; font-family: var(--font-display); font-size: 1.2rem; font-weight: 700; }
.formation span.d { color: var(--ink-2); font-size: 15px; }

/* Certifications */
.certs { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 20px; counter-reset: c; }
.cert { background: var(--surface); border: 1px solid var(--line); border-radius: 10px; overflow: hidden; display: flex; flex-direction: column; min-width: 0; }
.cert-img { display: block; width: 100%; border: 0; padding: 0; background: var(--ti-soft); cursor: zoom-in; border-bottom: 1px solid var(--line); }
.cert-img img { display: block; width: 100%; height: auto; }
.cert-body { padding: 18px 20px 22px; display: flex; flex-direction: column; gap: 10px; flex: 1; }
.cert-date { font-family: var(--font-mono); font-size: 12.5px; letter-spacing: .08em; text-transform: uppercase; color: var(--ti); }
.cert h3 { font-size: 1.25rem; font-weight: 700; }
.cert ul { display: grid; gap: 6px; font-size: 15px; color: var(--ink-2); }
.cert li { padding-left: 16px; position: relative; }
.cert li::before { content: ""; position: absolute; left: 0; top: .72em; width: 7px; height: 2px; background: var(--ti); }
.path { display: flex; align-items: center; gap: 12px; margin-bottom: 20px; font-family: var(--font-mono); font-size: 13px; color: var(--ink-2); flex-wrap: wrap; }
.path i { flex: 0 0 28px; height: 2px; background: linear-gradient(90deg, var(--ti), var(--ge-fill)); }
.note { margin-top: 18px; font-size: 14.5px; color: var(--ink-2); }

/* Expériences */
.xp { display: grid; gap: 0; }
.xp-item { display: grid; grid-template-columns: minmax(0, 3fr) minmax(0, 9fr); gap: clamp(12px, 3vw, 40px); padding-block: 28px; border-top: 1px solid var(--line); }
.xp-item:first-child { border-top: 0; padding-top: 0; }
.xp-when { font-family: var(--font-mono); font-size: 13.5px; color: var(--ink-2); line-height: 1.5; }
.xp-when b { display: block; color: var(--ink); font-weight: 500; }
.xp h3 { font-size: 1.45rem; font-weight: 700; }
.xp .org { margin-top: 2px; color: var(--ink-2); font-weight: 500; }
.xp ul { margin-top: 14px; display: grid; gap: 7px; max-width: 46em; }
.xp li { padding-left: 18px; position: relative; }
.xp li::before { content: ""; position: absolute; left: 0; top: .72em; width: 8px; height: 2px; background: var(--ge-fill); }
.xp .chips { margin-top: 16px; }

/* Postes visés */
.roles { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 16px; }
.role { background: var(--surface); border: 1px solid var(--line); border-radius: 10px; padding: 24px; min-width: 0; }
.role h3 { font-size: 1.3rem; font-weight: 700; }
.role .why { margin-top: 6px; color: var(--ink-2); font-size: 15.5px; }
.role ul { margin-top: 16px; display: grid; gap: 8px; }
.role li { display: flex; gap: 10px; align-items: baseline; font-size: 15.5px; }
.dot { flex: 0 0 9px; height: 9px; border-radius: 50%; transform: translateY(-1px); }
.dot.ti { background: var(--ti); }
.dot.ge { background: var(--ge-fill); }
.dot.both { background: linear-gradient(90deg, var(--ti) 50%, var(--ge-fill) 50%); }
.legend { display: flex; flex-wrap: wrap; gap: 6px 22px; margin-bottom: 20px; font-size: 14.5px; color: var(--ink-2); }
.legend span { display: inline-flex; align-items: center; gap: 8px; }

/* Contact */
.contact .wrap { display: grid; grid-template-columns: minmax(0, 7fr) minmax(0, 5fr); gap: clamp(24px, 5vw, 64px); align-items: end; }
.contact h2 { font-size: clamp(2.2rem, 5.4vw, 4rem); font-weight: 800; }
.contact p.sub { margin-top: 16px; color: var(--ink-2); max-width: 32em; }
.mailbox { background: var(--surface); border: 1px solid var(--line); border-radius: 10px; padding: 22px; min-width: 0; }
.mail { display: block; margin-top: 8px; font-family: var(--font-mono); font-size: clamp(14px, 2.6vw, 17px); word-break: break-all; user-select: all; }
.mailbox .actions { margin-top: 18px; }
.status { min-height: 1.4em; margin-top: 10px; font-size: 14px; color: var(--ti); }
footer { border-top: 1px solid var(--line); padding-block: 28px; font-size: 14.5px; color: var(--ink-2); }
footer .wrap { display: flex; flex-wrap: wrap; justify-content: space-between; gap: 8px 24px; }

/* Visionneuse */
dialog { border: 0; padding: 0; background: transparent; max-width: min(94vw, 1100px); width: 100%; }
dialog::backdrop { background: rgba(5, 12, 18, .82); }
dialog .frame { position: relative; }
dialog img { display: block; width: 100%; height: auto; border-radius: 8px; background: #fff; }
dialog .close { position: absolute; top: 10px; right: 10px; font: 600 14px var(--font-body); padding: 8px 14px; border-radius: 8px; border: 0; background: var(--ink); color: var(--bg); cursor: pointer; }

/* Illustration du héros */
.t-link { stroke: var(--ti); stroke-width: 1.6; fill: none; opacity: .55; }
.t-flow { stroke: var(--ti); stroke-width: 1.8; fill: none; stroke-dasharray: 5 7; animation: flow 2.4s linear infinite; }
.t-node { fill: var(--ti); transform-box: fill-box; transform-origin: center; animation: pulse 3.2s ease-in-out infinite; }
.g-bar { fill: var(--ge-fill); }
.g-grid { stroke: var(--line); stroke-width: 1; }
.g-flow { stroke: var(--ge-fill); stroke-width: 1.8; fill: none; stroke-dasharray: 5 7; animation: flow 2.4s linear infinite; }
.svg-label { font-family: var(--font-mono); font-size: 12px; letter-spacing: .12em; }
@keyframes flow { to { stroke-dashoffset: -48; } }
@keyframes pulse { 0%, 100% { transform: scale(1); } 50% { transform: scale(1.35); } }
.d2 { animation-delay: .6s; } .d3 { animation-delay: 1.2s; } .d4 { animation-delay: 1.8s; } .d5 { animation-delay: 2.4s; }

@media (max-width: 900px) {
  .hero .wrap, .section-head, .contact .wrap { grid-template-columns: minmax(0, 1fr); }
  .hero-art { justify-self: start; max-width: 440px; }
  .facts { grid-template-columns: repeat(2, minmax(0, 1fr)); }
  .bridge, .certs { grid-template-columns: minmax(0, 1fr); }
  .roles { grid-template-columns: minmax(0, 1fr); }
  .xp-item { grid-template-columns: minmax(0, 1fr); gap: 6px; }
  .certs { max-width: 560px; }
}
@media (max-width: 560px) {
  .top .wrap { flex-direction: column; align-items: flex-start; gap: 4px; }
  .nav { width: 100%; margin-left: -10px; }
  .formation { grid-template-columns: minmax(0, 1fr); }
}
@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after { animation: none !important; transition: none !important; scroll-behavior: auto !important; }
}
</style>

<header class="top">
  <div class="wrap">
    <a class="brand" href="#haut" aria-label="Ibrahima Kebe, haut de page"><span>Ibrahima</span> <span>Kebe</span></a>
    <nav class="nav" aria-label="Sections">
      <a href="#profil">Profil</a>
      <a href="#certifications">Certifications</a>
      <a href="#experience">Expérience</a>
      <a href="#postes">Postes visés</a>
      <a href="#contact">Contact</a>
    </nav>
  </div>
</header>

<main id="haut">
  <section class="hero">
    <div class="wrap">
      <div>
        <p class="eyebrow">Ibrahima Ben Mady Kebe · Montréal, QC</p>
        <h1>La <span class="ti-text">technique</span> et la <span class="ge-text">gestion</span>, dans un seul profil.</h1>
        <p class="lede">Je configure des réseaux Cisco et je coordonne des opérations. Formé en informatique appliquée à la gestion, titulaire d'un MBA, je relie ce que les systèmes permettent à ce que l'équipe doit livrer.</p>
        <div class="actions">
          <a class="btn primary" href="#certifications">Voir mes certifications</a>
          <a class="btn" href="#contact">Me contacter</a>
        </div>
      </div>
      <div class="hero-art">
        <svg viewBox="0 0 520 380" role="img" aria-labelledby="art-t art-d">
          <title id="art-t">Un réseau à gauche, un calendrier de projet à droite, reliés par un point central</title>
          <desc id="art-d">Des nœuds de réseau bleus à gauche et des barres de planification ambre à droite, reliés par un nœud central.</desc>
          <defs>
            <linearGradient id="core" x1="0" y1="0" x2="1" y2="0">
              <stop offset="0" style="stop-color: var(--ti)"/>
              <stop offset="1" style="stop-color: var(--ge-fill)"/>
            </linearGradient>
          </defs>
          <!-- réseau -->
          <path class="t-link" d="M60 70 L150 44 L190 140 L60 130 Z M190 140 L110 230 L60 130 M110 230 L200 290 L190 140 M60 130 L40 220 L110 230"/>
          <path class="t-flow" d="M190 140 L254 190 M200 290 L254 190"/>
          <circle class="t-node" cx="60" cy="70" r="7"/>
          <circle class="t-node d2" cx="150" cy="44" r="7"/>
          <circle class="t-node d3" cx="190" cy="140" r="9"/>
          <circle class="t-node d4" cx="60" cy="130" r="7"/>
          <circle class="t-node d5" cx="110" cy="230" r="8"/>
          <circle class="t-node d2" cx="200" cy="290" r="7"/>
          <circle class="t-node d3" cx="40" cy="220" r="6"/>
          <!-- planning -->
          <g class="g-grid"><path d="M330 56 V330 M380 56 V330 M430 56 V330 M480 56 V330"/></g>
          <rect class="g-bar" x="316" y="64" width="110" height="18" rx="4"/>
          <rect class="g-bar" x="352" y="104" width="128" height="18" rx="4" opacity=".85"/>
          <rect class="g-bar" x="330" y="144" width="70" height="18" rx="4"/>
          <rect class="g-bar" x="392" y="184" width="96" height="18" rx="4" opacity=".85"/>
          <rect class="g-bar" x="346" y="224" width="118" height="18" rx="4"/>
          <rect class="g-bar" x="318" y="264" width="86" height="18" rx="4" opacity=".85"/>
          <path class="g-flow" d="M266 190 L316 190"/>
          <!-- pont -->
          <circle cx="260" cy="190" r="22" fill="none" stroke="url(#core)" stroke-width="2" opacity=".5"/>
          <circle cx="260" cy="190" r="12" fill="url(#core)"/>
          <text class="svg-label" x="40" y="350" style="fill: var(--ti)">TI</text>
          <text class="svg-label" x="316" y="350" style="fill: var(--ge)">GESTION</text>
        </svg>
      </div>
    </div>
    <div class="wrap">
      <dl class="facts">
        <div><dt>Formation</dt><dd>Bac. informatique appliquée à la gestion, MBA</dd></div>
        <div><dt>Certifications</dt><dd>3 formations Cisco Networking Academy</dd></div>
        <div><dt>Langues</dt><dd>Français et anglais</dd></div>
        <div><dt>Recherche</dt><dd>Poste en TI, réseau ou coordination de projets</dd></div>
      </dl>
    </div>
  </section>

  <section class="section" id="profil">
    <div class="wrap">
      <div class="section-head">
        <div>
          <p class="eyebrow">Profil hybride</p>
          <h2>Ce que je fais côté TI, côté gestion, et là où les deux se rejoignent.</h2>
        </div>
        <p>Les trois colonnes montrent mes compétences réelles. Filtre pour voir chaque côté. La colonne du centre regroupe ce qui sert aux deux : c'est là que mon profil se distingue.</p>
      </div>

      <div class="filters" role="group" aria-label="Filtrer les compétences">
        <button class="filter" type="button" data-f="all" aria-pressed="true">Tout voir</button>
        <button class="filter" type="button" data-f="ti" aria-pressed="false">Côté TI</button>
        <button class="filter" type="button" data-f="both" aria-pressed="false">Les deux</button>
        <button class="filter" type="button" data-f="ge" aria-pressed="false">Côté gestion</button>
      </div>

      <div class="bridge">
        <div class="col" data-kind="ti">
          <h3>Côté TI</h3>
          <p class="sub">Réseaux, systèmes et support</p>
          <div class="chips">
            <span class="chip ti">Cisco CLI</span>
            <span class="chip ti">TCP/IP</span>
            <span class="chip ti">IPv4 / IPv6</span>
            <span class="chip ti">Sous-réseaux</span>
            <span class="chip ti">VLAN et trunk</span>
            <span class="chip ti">Routage inter-VLAN</span>
            <span class="chip ti">OSPF</span>
            <span class="chip ti">STP</span>
            <span class="chip ti">EtherChannel</span>
            <span class="chip ti">DHCP</span>
            <span class="chip ti">NAT</span>
            <span class="chip ti">ACL</span>
            <span class="chip ti">HSRP</span>
            <span class="chip ti">Dépannage matériel</span>
            <span class="chip ti">Installation de systèmes</span>
            <span class="chip ti">Support aux utilisateurs</span>
          </div>
        </div>
        <div class="col" data-kind="both">
          <h3>Les deux</h3>
          <p class="sub">Ce qui relie les systèmes et les équipes</p>
          <div class="chips">
            <span class="chip both">Excel avancé</span>
            <span class="chip both">Office 365</span>
            <span class="chip both">Compilation de données</span>
            <span class="chip both">Validation de données</span>
            <span class="chip both">Systèmes d'inventaire</span>
            <span class="chip both">Documentation rigoureuse</span>
            <span class="chip both">Rapports et présentations</span>
            <span class="chip both">Analyse de processus</span>
            <span class="chip both">Français / English</span>
          </div>
        </div>
        <div class="col" data-kind="ge">
          <h3>Côté gestion</h3>
          <p class="sub">Projets, équipes et opérations</p>
          <div class="chips">
            <span class="chip ge">Suivi de projets</span>
            <span class="chip ge">Calendriers de projet</span>
            <span class="chip ge">Validation de livrables</span>
            <span class="chip ge">Feuilles de temps et horaires</span>
            <span class="chip ge">Coordination d'équipes</span>
            <span class="chip ge">Gestion d'événements</span>
            <span class="chip ge">Facturation mensuelle</span>
            <span class="chip ge">Analyse de dossiers de crédit</span>
            <span class="chip ge">Rédaction professionnelle</span>
            <span class="chip ge">MBA</span>
          </div>
        </div>
      </div>

      <div class="formation">
        <div>
          <span class="eyebrow">2022 – 2025</span>
          <strong>MBA, Master of Business Administration</strong>
          <span class="d">Administration des affaires</span>
        </div>
        <div>
          <span class="eyebrow">2017 – 2020</span>
          <strong>Bac. en informatique appliquée à la gestion</strong>
          <span class="d">Systèmes informatiques et gestion de données</span>
        </div>
      </div>
    </div>
  </section>

  <section class="section" id="certifications">
    <div class="wrap">
      <div class="section-head">
        <div>
          <p class="eyebrow">Certifications</p>
          <h2>Du poste de travail au réseau d'entreprise.</h2>
        </div>
        <p>Trois formations Cisco Networking Academy, suivies dans cet ordre entre 2018 et 2019. Chaque étape ajoute une couche à la précédente. Clique sur un certificat pour l'agrandir.</p>
      </div>

      <div class="path" aria-hidden="true">
        <span>Matériel et systèmes</span><i></i><span>Réseau local</span><i></i><span>Réseau d'entreprise</span>
      </div>

      <div class="certs">
        <article class="cert">
          <button class="cert-img" type="button" data-src="certificats/it-essentials.png" data-alt="Certificat IT Essentials : PC Hardware and Software" aria-label="Agrandir le certificat IT Essentials">
            <img src="certificats/it-essentials.png" alt="Certificat IT Essentials : PC Hardware and Software" loading="lazy">
          </button>
          <div class="cert-body">
            <span class="cert-date">25 avril 2018</span>
            <h3>IT Essentials : PC Hardware and Software</h3>
            <ul>
              <li>Assemblage, diagnostic et dépannage de matériel</li>
              <li>Installation et configuration de systèmes d'exploitation</li>
              <li>Support de premier niveau et notions de sécurité</li>
            </ul>
          </div>
        </article>
        <article class="cert">
          <button class="cert-img" type="button" data-src="certificats/ccna-introduction-to-networks.png" data-alt="Certificat CCNA R&S : Introduction to Networks" aria-label="Agrandir le certificat CCNA Introduction to Networks">
            <img src="certificats/ccna-introduction-to-networks.png" alt="Certificat CCNA R&S : Introduction to Networks" loading="lazy">
          </button>
          <div class="cert-body">
            <span class="cert-date">27 juin 2018</span>
            <h3>CCNA R&amp;S : Introduction to Networks</h3>
            <ul>
              <li>Modèles OSI et TCP/IP, adressage IPv4 et IPv6</li>
              <li>Sous-réseaux, Ethernet et commutation</li>
              <li>Configuration initiale de routeurs et commutateurs Cisco</li>
            </ul>
          </div>
        </article>
        <article class="cert">
          <button class="cert-img" type="button" data-src="certificats/ccna-routing-and-switching-essentials.png" data-alt="Certificat CCNA R&S : Routing and Switching Essentials" aria-label="Agrandir le certificat CCNA Routing and Switching Essentials">
            <img src="certificats/ccna-routing-and-switching-essentials.png" alt="Certificat CCNA R&S : Routing and Switching Essentials" loading="lazy">
          </button>
          <div class="cert-body">
            <span class="cert-date">25 mars 2019</span>
            <h3>CCNA R&amp;S : Routing and Switching Essentials</h3>
            <ul>
              <li>VLAN, trunk et routage inter-VLAN</li>
              <li>OSPF, STP, EtherChannel et HSRP</li>
              <li>DHCP, NAT et listes de contrôle d'accès</li>
            </ul>
          </div>
        </article>
      </div>
      <p class="note">Attestations de cours délivrées par Cisco Networking Academy.</p>
    </div>
  </section>

  <section class="section" id="experience">
    <div class="wrap">
      <div class="section-head">
        <div>
          <p class="eyebrow">Expérience</p>
          <h2>Quatre rôles où j'ai analysé, coordonné et documenté.</h2>
        </div>
        <p>Chaque poste m'a appris à travailler avec des données fiables, des équipes différentes et des échéances précises. Ce sont les mêmes réflexes que j'applique en TI.</p>
      </div>

      <div class="xp">
        <article class="xp-item">
          <div class="xp-when"><b>Fév. – Juin 2026</b>Magna Stainless et Aluminium</div>
          <div>
            <h3>Analyste traitement et entrée de données</h3>
            <p class="org">Magna Stainless et Aluminium</p>
            <ul>
              <li>Réception de l'inventaire et vérification quotidienne de la conformité.</li>
              <li>Mise à jour quotidienne des systèmes de gestion d'inventaire et de suivi.</li>
              <li>Vérification des certificats de conformité et traitement des documents de réception et d'expédition.</li>
              <li>Collaboration avec le crédit, la comptabilité, l'entrepôt et la livraison.</li>
            </ul>
            <div class="chips"><span class="chip both">Données</span><span class="chip both">Systèmes d'inventaire</span><span class="chip ge">Conformité</span></div>
          </div>
        </article>
        <article class="xp-item">
          <div class="xp-when"><b>Jan. – Juil. 2025</b>Projet UQAM / Hôtel Monville</div>
          <div>
            <h3>Analyste projet, optimisation des opérations</h3>
            <p class="org">Projet UQAM / Hôtel Monville</p>
            <ul>
              <li>Suivi administratif complet de projets hôteliers et gestion documentaire méthodique.</li>
              <li>Compilation de données pour des rapports détaillés.</li>
              <li>Création de présentations pour appuyer la direction.</li>
              <li>Gestion des calendriers de projet, des feuilles de temps et validation des livrables.</li>
            </ul>
            <div class="chips"><span class="chip ge">Suivi de projet</span><span class="chip both">Rapports</span><span class="chip both">Présentations</span></div>
          </div>
        </article>
        <article class="xp-item">
          <div class="xp-when"><b>Juin 2022 – Mars 2026</b>Hôtel Monville, Montréal</div>
          <div>
            <h3>Événementiel banquet</h3>
            <p class="org">Hôtel Monville</p>
            <ul>
              <li>Gestion administrative d'événements corporatifs complexes, avec suivi des détails.</li>
              <li>Coordination d'équipes multidisciplinaires, des feuilles de temps et des horaires.</li>
              <li>Rédaction de correspondances, de rapports et de mémos liés aux opérations.</li>
              <li>Soutien aux directeurs et aux superviseurs, préparation des commandes d'équipement.</li>
            </ul>
            <div class="chips"><span class="chip ge">Coordination d'équipes</span><span class="chip ge">Gestion d'événements</span><span class="chip ge">Rédaction</span></div>
          </div>
        </article>
        <article class="xp-item">
          <div class="xp-when"><b>Sept. 2021 – Mai 2022</b>Bank of Africa</div>
          <div>
            <h3>Analyste crédit junior</h3>
            <p class="org">Bank of Africa</p>
            <ul>
              <li>Analyse de dossiers clients et montage de dossiers de crédit.</li>
              <li>Vérification de l'exactitude des informations critiques.</li>
              <li>Collaboration avec les équipes internes pour valider les dossiers et appuyer la décision.</li>
            </ul>
            <div class="chips"><span class="chip ge">Analyse de dossiers</span><span class="chip both">Validation de données</span></div>
          </div>
        </article>
      </div>
    </div>
  </section>

  <section class="section" id="postes">
    <div class="wrap">
      <div class="section-head">
        <div>
          <p class="eyebrow">Postes visés</p>
          <h2>Où mon profil s'applique le mieux.</h2>
        </div>
        <p>Pour chaque type de poste, voici ce que j'apporte et de quel côté ça vient.</p>
      </div>

      <div class="legend" aria-label="Légende">
        <span><i class="dot ti"></i>Côté TI</span>
        <span><i class="dot both"></i>Les deux</span>
        <span><i class="dot ge"></i>Côté gestion</span>
      </div>

      <div class="roles">
        <article class="role">
          <h3>Technicien en support informatique</h3>
          <p class="why">Résoudre les problèmes des utilisateurs et garder les postes en état de marche.</p>
          <ul>
            <li><i class="dot ti"></i>IT Essentials : matériel, systèmes, dépannage</li>
            <li><i class="dot ti"></i>Support aux utilisateurs et installation de postes</li>
            <li><i class="dot both"></i>Documentation rigoureuse des interventions</li>
            <li><i class="dot ge"></i>Service à la clientèle, en français et en anglais</li>
          </ul>
        </article>
        <article class="role">
          <h3>Technicien réseau junior</h3>
          <p class="why">Configurer, surveiller et dépanner des réseaux locaux et d'entreprise.</p>
          <ul>
            <li><i class="dot ti"></i>CCNA R&amp;S : VLAN, OSPF, STP, DHCP, NAT, ACL</li>
            <li><i class="dot ti"></i>Configuration de routeurs et commutateurs Cisco</li>
            <li><i class="dot both"></i>Documentation et suivi des configurations</li>
            <li><i class="dot ge"></i>Coordination avec les équipes et les fournisseurs</li>
          </ul>
        </article>
        <article class="role">
          <h3>Coordonnateur de projets TI</h3>
          <p class="why">Tenir les échéances d'un projet en comprenant ce que la technique exige.</p>
          <ul>
            <li><i class="dot ge"></i>MBA et suivi de projet (projet UQAM / Hôtel Monville)</li>
            <li><i class="dot ge"></i>Calendriers, feuilles de temps, validation des livrables</li>
            <li><i class="dot both"></i>Rapports et présentations pour la direction</li>
            <li><i class="dot ti"></i>Bases réseau et systèmes pour dialoguer avec les équipes TI</li>
          </ul>
        </article>
        <article class="role">
          <h3>Analyste opérations et données</h3>
          <p class="why">Fiabiliser l'information qui circule entre les systèmes et les départements.</p>
          <ul>
            <li><i class="dot both"></i>Excel avancé, compilation et validation de données</li>
            <li><i class="dot both"></i>Systèmes d'inventaire et de suivi (Magna)</li>
            <li><i class="dot ge"></i>Analyse de dossiers et de processus</li>
            <li><i class="dot ti"></i>Formation en informatique appliquée à la gestion</li>
          </ul>
        </article>
      </div>
    </div>
  </section>

  <section class="section contact" id="contact">
    <div class="wrap">
      <div>
        <p class="eyebrow">Contact</p>
        <h2>Un poste à pourvoir ? Écrivez-moi.</h2>
        <p class="sub">Je réponds en français ou en anglais. Je suis à Montréal et je cherche un poste où la technique et la coordination travaillent ensemble.</p>
      </div>
      <div class="mailbox">
        <span class="eyebrow">Courriel</span>
        <span class="mail" id="mail">benmadykebe@gmail.com</span>
        <div class="actions">
          <button class="btn primary" type="button" id="copy">Copier l'adresse</button>
          <a class="btn" href="mailto:benmadykebe@gmail.com">Écrire un courriel</a>
        </div>
        <p class="status" id="status" role="status" aria-live="polite"></p>
      </div>
    </div>
  </section>
</main>

<footer>
  <div class="wrap">
    <span>Ibrahima Ben Mady Kebe</span>
    <span>Montréal, QC · Français et anglais</span>
  </div>
</footer>

<dialog id="lb" aria-label="Certificat agrandi">
  <div class="frame">
    <img id="lb-img" alt="">
    <button class="close" type="button" id="lb-close">Fermer</button>
  </div>
</dialog>

<script>
(function () {
  // Filtre des compétences
  var filters = document.querySelectorAll('.filter');
  var cols = document.querySelectorAll('.col');
  filters.forEach(function (btn) {
    btn.addEventListener('click', function () {
      var f = btn.getAttribute('data-f');
      filters.forEach(function (b) { b.setAttribute('aria-pressed', b === btn ? 'true' : 'false'); });
      cols.forEach(function (c) {
        var dim = f !== 'all' && c.getAttribute('data-kind') !== f;
        c.setAttribute('data-dim', dim ? 'true' : 'false');
      });
    });
  });

  // Visionneuse de certificats
  var dlg = document.getElementById('lb');
  var big = document.getElementById('lb-img');
  document.querySelectorAll('.cert-img').forEach(function (b) {
    b.addEventListener('click', function () {
      big.src = b.getAttribute('data-src');
      big.alt = b.getAttribute('data-alt') || '';
      if (dlg.showModal) { dlg.showModal(); } else { dlg.setAttribute('open', ''); }
    });
  });
  function closeLb() { if (dlg.close) { dlg.close(); } else { dlg.removeAttribute('open'); } }
  document.getElementById('lb-close').addEventListener('click', closeLb);
  dlg.addEventListener('click', function (e) { if (e.target === dlg) { closeLb(); } });

  // Copie de l'adresse
  var status = document.getElementById('status');
  var mail = document.getElementById('mail');
  function selectMail() {
    var r = document.createRange(); r.selectNodeContents(mail);
    var s = window.getSelection(); s.removeAllRanges(); s.addRange(r);
  }
  document.getElementById('copy').addEventListener('click', function () {
    var done = function () { status.textContent = 'Adresse copiée.'; };
    var fail = function () { selectMail(); status.textContent = 'Adresse sélectionnée : copie-la avec Ctrl+C.'; };
    try {
      if (navigator.clipboard && navigator.clipboard.writeText) {
        navigator.clipboard.writeText(mail.textContent.trim()).then(done, fail);
      } else { fail(); }
    } catch (e) { fail(); }
  });
})();
</script>

</body></html>
