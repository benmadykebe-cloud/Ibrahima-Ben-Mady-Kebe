// build-assets.js
// Génère les animations SVG du README (en-têtes, bandeau défilant, cartes, terminal, séparateur, vague).
// Utilisation : node build-assets.js   →   écrit les fichiers dans ./assets
// Aucune dépendance. Modifie la section STYLE et CONTENU puis relance le script.

const fs = require('fs');
const path = require('path');

const OUT = path.join(__dirname, 'assets');
fs.mkdirSync(OUT, { recursive: true });

/* ============================== STYLE ============================== */
const T = {
  navy900: '#0B2A40',
  navy700: '#1A5276',
  blue500: '#2E86C1',
  sky300: '#5DADE2',
  sky200: '#85C1E9',
  sky100: '#AED6F1',
  ice: '#D6EAF8',
  term: '#0D1117',
  termText: '#E6EDF3',
  font: 'Arial, Helvetica, sans-serif',
  mono: "'Courier New', Courier, monospace",
};

/* ============================= CONTENU ============================= */
const CONTENT = {
  sections: [
    ['apropos', 'À propos'],
    ['competences', 'Compétences'],
    ['certifications', 'Certifications'],
    ['projets', 'Projets'],
    ['parcours', 'Parcours'],
    ['contact', 'Contact'],
  ],
  marquee: [
    'Cisco CLI', 'TCP/IP', 'IPv4/IPv6', 'VLAN', 'OSPF', 'STP', 'EtherChannel',
    'DHCP', 'NAT', 'ACL', 'HSRP', 'Excel avancé', 'PowerPoint', 'Office 365',
    'Saisie et validation de données', 'Suivi de projets', 'Bilingue FR/EN',
  ],
  stats: [
    ['3', 'certifications', 'Cisco Networking Academy'],
    ['2', 'diplômes', 'Bac. + MBA'],
    ['4', 'expériences', 'analyse · opérations · projets'],
    ['2', 'langues', 'français · anglais'],
  ],
  terminal: [
    'Router> enable',
    'Router# configure terminal',
    'Router(config)# router ospf 1',
    'Router(config-router)# network 192.168.1.0 0.0.0.255 area 0',
    'Router(config-router)# end',
  ],
  terminalTitle: 'Terminal · Cisco CLI',
  footer: 'Montréal, QC  ·  Disponible en français et en anglais',
};

/* ============================ OUTILS =============================== */
const REDUCED = '@media (prefers-reduced-motion: reduce){*{animation:none !important}}';
const esc = (s) => s.replace(/&/g, '&amp;').replace(/</g, '&lt;').replace(/>/g, '&gt;');
const f = (n) => Number(n.toFixed(2));
const svg = (w, h, label, body) =>
  `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 ${w} ${h}" width="${w}" height="${h}" role="img" aria-label="${esc(label)}">\n${body}\n</svg>\n`;
const write = (name, content) => {
  fs.writeFileSync(path.join(OUT, name), content);
  console.log('OK', name);
};

/* ====================== 1. EN-TÊTES DE SECTIONS ==================== */
const sectionSvg = (title) =>
  svg(1200, 64, title, `
<defs>
  <linearGradient id="g" x1="0" y1="0" x2="1" y2="0">
    <stop offset="0" stop-color="${T.navy900}"/><stop offset="1" stop-color="${T.navy700}"/>
  </linearGradient>
  <linearGradient id="sw" x1="0" y1="0" x2="1" y2="0">
    <stop offset="0" stop-color="#fff" stop-opacity="0"/>
    <stop offset=".5" stop-color="#fff" stop-opacity=".16"/>
    <stop offset="1" stop-color="#fff" stop-opacity="0"/>
  </linearGradient>
  <clipPath id="c"><rect width="1200" height="64" rx="12"/></clipPath>
  <style>
    .t { font-family: ${T.font}; font-size: 30px; font-weight: 700; fill: #fff; animation: in .7s ease-out backwards; }
    .bar { fill: ${T.sky300}; transform-box: fill-box; transform-origin: center; animation: grow .7s ease-out backwards; }
    .dot { fill: ${T.sky200}; animation: blink 2s ease-in-out infinite; }
    .sweep { animation: sweep 5s ease-in-out infinite; }
    @keyframes in { from { opacity: 0; transform: translateX(-18px); } }
    @keyframes grow { from { transform: scaleY(0); } }
    @keyframes blink { 0%, 100% { opacity: 1; } 50% { opacity: .25; } }
    @keyframes sweep { 0% { transform: translateX(0); } 60%, 100% { transform: translateX(1500px); } }
    ${REDUCED}
  </style>
</defs>
<g clip-path="url(#c)">
  <rect width="1200" height="64" fill="url(#g)"/>
  <rect class="sweep" x="-260" width="260" height="64" fill="url(#sw)"/>
</g>
<rect class="bar" x="22" y="14" width="6" height="36" rx="3"/>
<circle class="dot" cx="1170" cy="32" r="5"/>
<text class="t" x="46" y="43">${esc(title)}</text>`);

CONTENT.sections.forEach(([id, title]) => write(`section-${id}.svg`, sectionSvg(title)));

/* ====================== 2. BANDEAU DÉFILANT ======================== */
const marqueeSvg = () => {
  const items = CONTENT.marquee;
  const gap = 14;
  const h = 38;
  const widths = items.map((s) => Math.round(s.length * 9.6 + 36));
  const total = widths.reduce((a, w) => a + w + gap, 0);
  const speed = 55; // pixels par seconde
  const row = (offset) => {
    let x = offset;
    return items
      .map((s, i) => {
        const w = widths[i];
        const g = `<g transform="translate(${x} 9)"><rect width="${w}" height="${h}" rx="19" fill="url(#p)" stroke="${T.sky300}" stroke-opacity=".55"/><text class="m" x="${f(w / 2)}" y="25" text-anchor="middle">${esc(s)}</text></g>`;
        x += w + gap;
        return g;
      })
      .join('');
  };
  return svg(1200, 56, 'Mots-clés : ' + items.join(', '), `
<defs>
  <linearGradient id="p" x1="0" y1="0" x2="1" y2="0">
    <stop offset="0" stop-color="${T.navy900}"/><stop offset="1" stop-color="${T.navy700}"/>
  </linearGradient>
  <linearGradient id="fm" x1="0" y1="0" x2="1" y2="0">
    <stop offset="0" stop-color="#000"/><stop offset=".06" stop-color="#fff"/>
    <stop offset=".94" stop-color="#fff"/><stop offset="1" stop-color="#000"/>
  </linearGradient>
  <mask id="fade"><rect width="1200" height="56" fill="url(#fm)"/></mask>
  <style>
    .m { font-family: ${T.font}; font-size: 16px; font-weight: 600; fill: #fff; }
    .row { animation: scroll ${f(total / speed)}s linear infinite; }
    @keyframes scroll { to { transform: translateX(-${total}px); } }
    ${REDUCED}
  </style>
</defs>
<g mask="url(#fade)"><g class="row">${row(0)}${row(total)}</g></g>`);
};
write('marquee.svg', marqueeSvg());

/* ====================== 3. CARTES DE CHIFFRES ====================== */
const statsSvg = () => {
  const cw = 285, gap = 20, h = 150;
  const cards = CONTENT.stats
    .map(([n, label, sub], i) => {
      const x = i * (cw + gap);
      return `<g class="card" style="animation-delay:${f(i * 0.15)}s" transform="translate(${x} 0)">
  <g class="fl" style="animation-delay:${f(i * 0.6)}s">
    <rect width="${cw}" height="${h - 10}" y="5" rx="16" fill="url(#cg)" stroke="${T.sky300}" stroke-opacity=".45"/>
    <text class="n" x="${cw / 2}" y="68" text-anchor="middle">${esc(n)}</text>
    <text class="l" x="${cw / 2}" y="100" text-anchor="middle">${esc(label)}</text>
    <text class="s" x="${cw / 2}" y="124" text-anchor="middle">${esc(sub)}</text>
  </g>
</g>`;
    })
    .join('\n');
  return svg(1200, h, CONTENT.stats.map((s) => `${s[0]} ${s[1]}`).join(', '), `
<defs>
  <linearGradient id="cg" x1="0" y1="0" x2="1" y2="1">
    <stop offset="0" stop-color="${T.navy900}"/><stop offset="1" stop-color="${T.navy700}"/>
  </linearGradient>
  <style>
    .n { font-family: ${T.font}; font-size: 54px; font-weight: 700; fill: #fff; }
    .l { font-family: ${T.font}; font-size: 20px; font-weight: 700; fill: ${T.sky100}; }
    .s { font-family: ${T.font}; font-size: 14px; fill: ${T.ice}; }
    .card { animation: rise .8s cubic-bezier(.2,.8,.2,1) backwards; }
    .fl { animation: float 5s ease-in-out infinite; }
    @keyframes rise { from { opacity: 0; transform: translateY(26px); } }
    @keyframes float { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-4px); } }
    ${REDUCED}
  </style>
</defs>
${cards}`);
};
write('stats.svg', statsSvg());

/* ====================== 4. TERMINAL CISCO ANIMÉ ==================== */
const terminalSvg = () => {
  const lines = CONTENT.terminal;
  const CW = 10.8; // largeur d'un caractère à 18 px en police monospace
  const LH = 34, X0 = 34, Y0 = 98, cycle = 18;
  const start = (i) => 0.8 + i * 2.7;
  const dur = (s) => Math.max(0.9, s.length * 0.045);
  let css = '';
  let covers = '';
  let texts = '';
  let lastEnd = 0;
  lines.forEach((s, i) => {
    const n = s.length;
    const W = Math.ceil(n * CW) + 8;
    const a = (start(i) / cycle) * 100;
    const b = ((start(i) + dur(s)) / cycle) * 100;
    lastEnd = b;
    css += `@keyframes tp${i} { 0%, ${f(a)}% { transform: scaleX(1); } ${f(b)}%, 95% { transform: scaleX(0); } 100% { transform: scaleX(1); } }\n    .k${i} { animation: tp${i} ${cycle}s steps(${n}, end) infinite; }\n    `;
    const m = s.match(/^(\S+[>#]\s)(.*)$/);
    const prompt = m ? m[1] : '';
    const cmd = m ? m[2] : s;
    const y = Y0 + i * LH;
    texts += `<text class="mono" x="${X0}" y="${y}" xml:space="preserve"><tspan fill="${T.sky300}">${esc(prompt)}</tspan><tspan fill="${T.termText}">${esc(cmd)}</tspan></text>\n`;
    covers += `<rect class="cv k${i}" x="${X0 - 2}" y="${y - 22}" width="${W}" height="30" fill="${T.term}"/>\n`;
  });
  const last = lines[lines.length - 1];
  const cx = f(X0 + last.length * CW + 4);
  const cy = Y0 + (lines.length - 1) * LH - 18;
  const H = Y0 + lines.length * LH - 6;
  return svg(1200, H, 'Animation : session en ligne de commande Cisco', `
<defs>
  <style>
    .mono { font-family: ${T.mono}; font-size: 18px; }
    .ttl { font-family: ${T.font}; font-size: 15px; fill: #8B949E; }
    .cv { transform: scaleX(0); transform-box: fill-box; transform-origin: 100% 50%; }
    ${css}.cur { opacity: 0; animation: curv ${cycle}s infinite; }
    .blink { animation: bl 1s steps(1) infinite; }
    @keyframes curv { 0%, ${f(lastEnd)}% { opacity: 0; } ${f(lastEnd + 0.1)}%, 95% { opacity: 1; } 100% { opacity: 0; } }
    @keyframes bl { 50% { opacity: 0; } }
    ${REDUCED}
  </style>
</defs>
<rect width="1200" height="${H}" rx="14" fill="${T.term}" stroke="${T.navy700}" stroke-width="2"/>
<path d="M0 14 a14 14 0 0 1 14 -14 H1186 a14 14 0 0 1 14 14 V44 H0 Z" fill="#161B22"/>
<circle cx="28" cy="22" r="6" fill="#FF5F56"/><circle cx="50" cy="22" r="6" fill="#FFBD2E"/><circle cx="72" cy="22" r="6" fill="#27C93F"/>
<text class="ttl" x="600" y="27" text-anchor="middle">${esc(CONTENT.terminalTitle)}</text>
${texts}${covers}<g class="cur"><rect class="blink" x="${cx}" y="${cy}" width="10" height="22" fill="${T.sky200}"/></g>`);
};
write('terminal.svg', terminalSvg());

/* ====================== 5. SÉPARATEUR ANIMÉ ======================== */
write(
  'divider.svg',
  svg(1200, 10, 'Séparateur', `
<defs>
  <linearGradient id="d" gradientUnits="userSpaceOnUse" x1="0" y1="0" x2="2400" y2="0">
    <stop offset="0" stop-color="${T.navy700}"/><stop offset=".25" stop-color="${T.sky300}"/>
    <stop offset=".5" stop-color="${T.navy700}"/><stop offset=".75" stop-color="${T.sky300}"/>
    <stop offset="1" stop-color="${T.navy700}"/>
  </linearGradient>
  <clipPath id="c"><rect y="2" width="1200" height="6" rx="3"/></clipPath>
  <style>
    .flow { animation: flow 6s linear infinite; }
    @keyframes flow { to { transform: translateX(-1200px); } }
    ${REDUCED}
  </style>
</defs>
<g clip-path="url(#c)"><rect class="flow" width="2400" height="10" fill="url(#d)"/></g>`)
);

/* ====================== 6. VAGUE DE PIED DE PAGE =================== */
const waveSvg = () => {
  const H = 140;
  const path_ = (base, amp, period, phase) => {
    const pts = [];
    for (let x = 0; x <= 1200 + period; x += 10) {
      pts.push(`${x} ${f(base + amp * Math.sin((2 * Math.PI * x) / period + phase))}`);
    }
    return `M${pts.join(' L')} L${1200 + period} ${H} L0 ${H} Z`;
  };
  const layers = [
    { base: 42, amp: 10, period: 600, phase: 0, fill: T.navy700, op: 0.25, dur: 16 },
    { base: 58, amp: 9, period: 400, phase: 1.2, fill: T.blue500, op: 0.35, dur: 12 },
    { base: 78, amp: 8, period: 300, phase: 2.4, fill: 'url(#solid)', op: 1, dur: 9 },
  ];
  let css = '';
  const paths = layers
    .map((L, i) => {
      css += `.w${i} { animation: w${i} ${L.dur}s linear infinite; }\n    @keyframes w${i} { to { transform: translateX(-${L.period}px); } }\n    `;
      return `<path class="w${i}" d="${path_(L.base, L.amp, L.period, L.phase)}" fill="${L.fill}" fill-opacity="${L.op}"/>`;
    })
    .join('\n');
  return svg(1200, H, 'Vague décorative', `
<defs>
  <linearGradient id="solid" x1="0" y1="0" x2="1" y2="0">
    <stop offset="0" stop-color="${T.navy900}"/><stop offset="1" stop-color="${T.navy700}"/>
  </linearGradient>
  <style>
    ${css}.ft { font-family: ${T.font}; font-size: 16px; fill: #fff; letter-spacing: .5px; }
    ${REDUCED}
  </style>
</defs>
${paths}
<text class="ft" x="600" y="124" text-anchor="middle">${esc(CONTENT.footer)}</text>`);
};
write('wave.svg', waveSvg());

console.log('\nTerminé : les fichiers sont dans le dossier assets/');
