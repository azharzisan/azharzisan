@import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&family=VT323:wght@400&display=swap'); \* { box-sizing: border-box; margin: 0; padding: 0; } .crt-wrap { background: #f0fff4; font-family: 'VT323', monospace; color: #1a5c2a; min-height: 520px; position: relative; overflow: hidden; border: 3px solid #4caf6e; box-shadow: inset 0 0 40px rgba(76,175,110,0.08); } .scanlines { pointer-events: none; position: absolute; inset: 0; background: repeating-linear-gradient( to bottom, transparent 0px, transparent 3px, rgba(76,175,110,0.07) 3px, rgba(76,175,110,0.07) 4px ); z-index: 10; } .crt-header { background: #e0f5e9; border-bottom: 2px solid #4caf6e; padding: 10px 18px; display: flex; align-items: center; gap: 10px; } .traffic-lights { display: flex; gap: 6px; } .dot { width: 10px; height: 10px; border-radius: 50%; } .dot-r { background: #ff6b6b; } .dot-y { background: #ffd166; } .dot-g { background: #06d6a0; } .crt-title-bar { font-family: 'Press Start 2P', monospace; font-size: 8px; color: #4caf6e; flex: 1; text-align: center; letter-spacing: 2px; } .crt-body { padding: 18px 22px 20px; } .pixel-gif { display: flex; justify-content: center; margin-bottom: 14px; } .hey-text { font-family: 'Press Start 2P', monospace; font-size: 12px; color: #216e39; line-height: 1.9; animation: glow 2.5s ease-in-out infinite alternate; } @keyframes glow { from { text-shadow: 0 0 2px #9be9a8; } to { text-shadow: 0 0 10px #40c463, 0 0 20px #9be9a855; } } .blink-cursor::after { content: '█'; animation: blink 1s step-end infinite; color: #40c463; font-size: 16px; } @keyframes blink { 0%,100%{opacity:1}50%{opacity:0} } .sub-text { font-size: 17px; color: #4caf6e; margin-top: 3px; letter-spacing: 1px; } .divider { border: none; border-top: 1px dashed #9be9a8; margin: 13px 0; } .section-head { font-family: 'Press Start 2P', monospace; font-size: 7px; color: #216e39; letter-spacing: 2px; margin-bottom: 9px; text-shadow: 0 0 4px #9be9a8; } .prompt-line { color: #40c463; font-size: 17px; margin-bottom: 3px; } .about-lines { font-size: 18px; color: #1a5c2a; line-height: 1.75; } .about-lines .label { color: #216e39; font-weight: bold; } .badges-row { display: flex; flex-wrap: wrap; gap: 8px; margin: 10px 0; } .badge { font-family: 'Press Start 2P', monospace; font-size: 6px; padding: 5px 8px; border: 2px solid; letter-spacing: 1px; cursor: default; transition: filter 0.15s; } .badge:hover { filter: brightness(1.3); } .badge-li { border-color: #0077B5; color: #0077B5; background: #e8f4fc; } .badge-yt { border-color: #cc0000; color: #cc0000; background: #fdf0f0; } .badge-tw { border-color: #1DA1F2; color: #1DA1F2; background: #eef8ff; } .badge-gh { border-color: #216e39; color: #216e39; background: #e0f5e9; } .tech-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(48px, 1fr)); gap: 7px; margin-top: 9px; } .tech-item { display: flex; flex-direction: column; align-items: center; gap: 4px; border: 1px solid #9be9a8; padding: 7px 3px 5px; background: #f0fff4; transition: border-color 0.2s, box-shadow 0.2s; } .tech-item:hover { border-color: #216e39; box-shadow: 0 0 6px #9be9a855; } .tech-icon { font-size: 20px; line-height: 1; } .tech-label { font-family: 'Press Start 2P', monospace; font-size: 5px; color: #4caf6e; text-align: center; line-height: 1.4; } /\* === GitHub-style contribution grid === \*/ .contrib-section { margin-top: 6px; } .contrib-labels { display: flex; gap: 0; margin-bottom: 3px; padding-left: 28px; } .contrib-month-label { font-family: 'Press Start 2P', monospace; font-size: 5px; color: #4caf6e; flex: 1; text-align: left; } .contrib-grid-wrap { display: flex; gap: 6px; } .day-labels { display: flex; flex-direction: column; gap: 2px; padding-top: 1px; } .day-label { font-family: 'Press Start 2P', monospace; font-size: 4.5px; color: #9be9a8; height: 10px; display: flex; align-items: center; } .contrib-grid { display: flex; gap: 2px; flex: 1; } .contrib-col { display: flex; flex-direction: column; gap: 2px; } .contrib-cell { width: 10px; height: 10px; border-radius: 2px; flex-shrink: 0; transition: opacity 0.1s; cursor: default; } .contrib-cell:hover { opacity: 0.75; } .c-0 { background: #ebedf0; } .c-1 { background: #9be9a8; } .c-2 { background: #40c463; } .c-3 { background: #30a14e; } .c-4 { background: #216e39; } .contrib-legend { display: flex; align-items: center; gap: 4px; margin-top: 6px; justify-content: flex-end; } .legend-label { font-family: 'Press Start 2P', monospace; font-size: 5px; color: #9be9a8; } .legend-cell { width: 10px; height: 10px; border-radius: 2px; } .stats-row { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 10px; margin-top: 10px; } .stat-card { border: 2px solid #9be9a8; padding: 10px 8px; text-align: center; background: #e0f5e9; } .stat-num { font-family: 'Press Start 2P', monospace; font-size: 14px; color: #216e39; display: block; margin-bottom: 4px; } .stat-lbl { font-size: 13px; color: #4caf6e; display: block; } .visitor-line { font-size: 13px; color: #9be9a8; margin-top: 14px; text-align: right; letter-spacing: 1px; } .visitor-count { color: #216e39; font-family: 'Press Start 2P', monospace; font-size: 8px; } .crt-footer { border-top: 1px solid #9be9a8; padding: 8px 22px; font-size: 13px; color: #4caf6e; display: flex; justify-content: space-between; background: #e0f5e9; }

README.md — PROFILE TERMINAL v1.0

\> hey there 👋

// frontend dev · builder · pixel pusher

* * *

\> cat about\_me.txt

\[ ABOUT ME \]

I'm Zisan from Bangladesh

🔭 Working on — React & Next.js apps

📚 Learning — Next.js, Tauri, SQLite

⚡ Free time — shipping side projects

* * *

\> ls socials/

\[ SOCIALS \]

LINKEDIN

YOUTUBE

TWITTER

GITHUB

* * *

\> ls tools/ --icons

\[ LANGUAGES + TOOLS \]

⚛React

▲Next.js

⚡Vite

🌀Tailwind

🔥Firebase

🐋Docker

☁AWS

🦀Rust

♻Go

🔷.NET

* * *

\> run contributions.sh --year 2024

\[ CONTRIBUTION GRAPH \]

Mon

Wed

Fri

less

more

* * *

\> run stats.sh

\[ MY STATS \]

0 commits

0 day streak

0 repos

visitors: 0

AzharZisan @ github \--:--:--

const WEEKS = 30; const grid = document.getElementById('contribGrid'); const monthLabels = document.getElementById('monthLabels'); const months = \['Jan','Feb','Mar','Apr','May','Jun','Jul','Aug','Sep','Oct','Nov','Dec'\]; const today = new Date(); function seededRand(seed) { let x = Math.sin(seed + 1) \* 10000; return x - Math.floor(x); } function getLevel(week, day) { const seed = week \* 7 + day; const r = seededRand(seed); if (r < 0.30) return 0; if (r < 0.50) return 1; if (r < 0.72) return 2; if (r < 0.87) return 3; return 4; } let lastMonth = -1; const labelSpans = \[\]; for (let w = 0; w < WEEKS; w++) { const col = document.createElement('div'); col.className = 'contrib-col'; const weekDate = new Date(today); weekDate.setDate(today.getDate() - (WEEKS - 1 - w) \* 7); const m = weekDate.getMonth(); if (m !== lastMonth) { labelSpans.push({ week: w, label: months\[m\] }); lastMonth = m; } for (let d = 0; d < 7; d++) { const cell = document.createElement('div'); cell.className = 'contrib-cell c-' + getLevel(w, d); col.appendChild(cell); } grid.appendChild(col); } labelSpans.forEach(({ week, label }) => { const span = document.createElement('span'); span.className = 'contrib-month-label'; span.textContent = label; span.style.marginLeft = week === 0 ? '0' : (week \* 12) + 'px'; monthLabels.appendChild(span); }); function animCount(el, target, duration) { let start = null; function step(ts) { if (!start) start = ts; const p = Math.min((ts - start) / duration, 1); el.textContent = Math.round(p \* target); if (p < 1) requestAnimationFrame(step); } requestAnimationFrame(step); } animCount(document.getElementById('commits'), 312, 1400); animCount(document.getElementById('streak'), 47, 1200); animCount(document.getElementById('repos'), 18, 1000); animCount(document.getElementById('visitorCount'), 2048, 2000); function updateClock() { const now = new Date(); const pad = n => String(n).padStart(2,'0'); document.getElementById('clock').textContent = pad(now.getHours()) + ':' + pad(now.getMinutes()) + ':' + pad(now.getSeconds()); } updateClock(); setInterval(updateClock, 1000);
