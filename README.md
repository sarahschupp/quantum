
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>World Quantum Day — Special Edition | April 14, 2026</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,300;0,9..144,700;0,9..144,900;1,9..144,300;1,9..144,700;1,9..144,900&family=Inter:wght@300;400;500;600&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">
<style>
/* ── RESET & ROOT ─────────────────────────────────────── */
*,*::before,*::after{margin:0;padding:0;box-sizing:border-box}
:root{
  --electric:#2BAAFF;
  --gold:#C9A94B;
  --rose:#B5102A;
  --cream:#F5EDD8;
  --navy:#0B1628;
  --cyan:#00E5FF;
  --jade:#00B886;
  --indigo:#1A0A4A;
}
html{font-size:18px;scroll-behavior:smooth}
body{font-family:'Inter',sans-serif;background:#050505;color:#f0f0f0;line-height:1.65;overflow-x:hidden}
section{position:relative;overflow:hidden}
img{display:block;max-width:100%}

/* ── COVER ────────────────────────────────────────────── */
#cover{
  min-height:100vh;
  background:#050505;
  display:grid;
  grid-template-columns:1fr 1fr;
  align-items:center;
  gap:0;
  padding:80px 80px 60px;
}
.cover-left{max-width:580px}
.issue-tag{
  font-family:'JetBrains Mono',monospace;
  font-size:.78rem;
  letter-spacing:.3em;
  text-transform:uppercase;
  color:var(--electric);
  margin-bottom:28px;
  display:block;
}
.cover-title{
  font-family:'Fraunces',serif;
  font-size:clamp(3.2rem,7vw,5.8rem);
  font-weight:900;
  line-height:.92;
  color:#fff;
  margin-bottom:36px;
}
.cover-title em{display:block;font-style:italic;color:var(--electric)}
.cover-sub{
  font-size:1.05rem;
  color:#888;
  line-height:1.75;
  max-width:420px;
  margin-bottom:48px;
}
.cover-dateline{
  font-family:'JetBrains Mono',monospace;
  font-size:.82rem;
  color:var(--gold);
  letter-spacing:.18em;
  text-transform:uppercase;
}
.cover-right{
  display:flex;
  justify-content:center;
  align-items:center;
}

/* Bloch sphere animation */
@keyframes spin-slow{from{transform:rotate(0deg)}to{transform:rotate(360deg)}}
@keyframes spin-med{from{transform:rotate(0deg)}to{transform:rotate(-360deg)}}
@keyframes pulse-dot{0%,100%{opacity:.5}50%{opacity:1}}
.orbit1{animation:spin-slow 12s linear infinite;transform-origin:200px 200px}
.orbit2{animation:spin-med 9s linear infinite;transform-origin:200px 200px}
.orbit3{animation:spin-slow 15s linear infinite;transform-origin:200px 200px}
.state-dot{animation:pulse-dot 2s ease-in-out infinite}
.state-dot-2{animation:pulse-dot 2s ease-in-out infinite .6s}

/* TOC strip */
#toc{
  background:#0e0e0e;
  border-top:1px solid #1e1e1e;
  border-bottom:1px solid #1e1e1e;
  padding:28px 80px;
  display:flex;
  gap:0;
  flex-wrap:wrap;
}
.toc-entry{
  display:flex;
  align-items:center;
  gap:10px;
  padding:8px 28px 8px 0;
  margin-right:28px;
  border-right:1px solid #222;
  text-decoration:none;
  color:#666;
  font-size:.82rem;
  letter-spacing:.04em;
  transition:color .2s;
  white-space:nowrap;
}
.toc-entry:last-child{border-right:none}
.toc-entry:hover{color:#fff}
.toc-n{
  font-family:'JetBrains Mono',monospace;
  color:var(--electric);
  font-size:.72rem;
}

/* ── STORY 1: HERO — QuEra Logical Qubits ────────────── */
#s1{
  min-height:100vh;
  background:#f0efea;
  color:#080808;
  display:grid;
  grid-template-rows:auto 1fr;
}
.s1-top{
  padding:56px 80px 0;
  display:flex;
  justify-content:space-between;
  align-items:center;
  border-bottom:2px solid #080808;
  padding-bottom:20px;
}
.story-tag{
  font-family:'JetBrains Mono',monospace;
  font-size:.72rem;
  letter-spacing:.28em;
  text-transform:uppercase;
  padding:5px 14px;
  border:1.5px solid currentColor;
}
.s1-body{
  padding:48px 80px 72px;
  display:grid;
  grid-template-columns:1.1fr 1fr;
  gap:72px;
  align-items:start;
}
.s1-hed{
  grid-column:1/-1;
  font-family:'Fraunces',serif;
  font-size:clamp(3.8rem,9vw,7.8rem);
  font-weight:900;
  line-height:.88;
  letter-spacing:-.02em;
  padding-bottom:40px;
  border-bottom:3px solid #080808;
  margin-bottom:40px;
}
.s1-hed .kicker{
  display:block;
  font-size:clamp(1.5rem,3vw,2.4rem);
  font-weight:300;
  font-style:italic;
  color:#444;
  margin-bottom:12px;
}
.s1-dek{
  font-size:1.25rem;
  line-height:1.65;
  color:#222;
  padding-left:24px;
  border-left:4px solid #080808;
  margin-bottom:36px;
}
.s1-body-text{
  font-size:1rem;
  line-height:1.8;
  color:#333;
}
.s1-body-text p+p{margin-top:1.2em}
.stat-card{
  background:#080808;
  color:#f0efea;
  padding:44px;
  align-self:start;
}
.stat-num{
  font-family:'Fraunces',serif;
  font-size:5.5rem;
  font-weight:900;
  line-height:1;
  color:var(--electric);
}
.stat-unit{
  font-family:'Fraunces',serif;
  font-size:2rem;
  font-weight:300;
  font-style:italic;
  color:#aaa;
  margin-top:4px;
}
.stat-desc{font-size:.9rem;color:#888;margin-top:16px;line-height:1.6}
.lattice-wrap{margin-top:40px}

/* ── STORY 2: LAB REPORT — Microsoft Topological ─────── */
#s2{
  min-height:100vh;
  background:var(--cream);
  color:#1a0f08;
}
.lab-header{
  padding:64px 80px 32px;
  border-bottom:1px solid #c8bda0;
  display:flex;
  justify-content:space-between;
  align-items:baseline;
}
.lab-hed{
  font-family:'Fraunces',serif;
  font-size:clamp(2.5rem,5.5vw,4.4rem);
  font-weight:700;
  line-height:1.05;
  max-width:700px;
}
.lab-meta{
  font-family:'JetBrains Mono',monospace;
  font-size:.75rem;
  color:#8a7b5c;
  text-align:right;
  line-height:2;
}
.lab-body{
  padding:48px 80px 80px;
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:64px;
  align-items:start;
}
.lab-col-left p:first-child::first-letter{
  font-family:'Fraunces',serif;
  font-size:5.5rem;
  font-weight:900;
  float:left;
  line-height:.8;
  margin:8px 16px 0 0;
  color:#8B1A1A;
}
.lab-col-left p{
  font-size:1rem;
  line-height:1.85;
  color:#2a1f14;
  margin-bottom:1.4em;
}
.lab-col-right{
  border-left:1px solid #c8bda0;
  padding-left:48px;
}
.lab-pullquote{
  font-family:'Fraunces',serif;
  font-size:1.65rem;
  font-weight:300;
  font-style:italic;
  line-height:1.4;
  color:#5a3e2b;
  margin:0 0 32px;
  padding-bottom:32px;
  border-bottom:1px solid #c8bda0;
}
.lab-aside{
  font-size:.9rem;
  color:#6b5a40;
  line-height:1.75;
  margin-top:32px;
}
.lab-aside strong{font-weight:600;color:#3a2814;display:block;margin-bottom:6px}
.braid-wrap{margin-top:40px;display:flex;justify-content:center}

/* ── STORY 3: BLUEPRINT — Google Willow ──────────────── */
#s3{
  min-height:100vh;
  background:#0d1117;
  color:var(--cyan);
  background-image:
    linear-gradient(rgba(0,229,255,.04) 1px,transparent 1px),
    linear-gradient(90deg,rgba(0,229,255,.04) 1px,transparent 1px);
  background-size:48px 48px;
}
.bp-header{
  padding:56px 80px 32px;
  border-bottom:1px solid rgba(0,229,255,.15);
  display:flex;
  align-items:center;
  gap:40px;
}
.bp-tag{
  font-family:'JetBrains Mono',monospace;
  font-size:.72rem;
  letter-spacing:.28em;
  text-transform:uppercase;
  padding:5px 14px;
  border:1px solid var(--cyan);
  color:var(--cyan);
}
.bp-tagline{
  font-family:'JetBrains Mono',monospace;
  font-size:.82rem;
  color:rgba(0,229,255,.5);
  letter-spacing:.1em;
}
.bp-hed{
  font-family:'Fraunces',serif;
  font-size:clamp(3rem,7vw,6rem);
  font-weight:900;
  line-height:.9;
  color:#fff;
  padding:48px 80px;
}
.bp-hed span{display:block;font-style:italic;color:var(--cyan)}
.bp-body{
  padding:0 80px 80px;
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:64px;
}
.bp-text p{
  font-family:'JetBrains Mono',monospace;
  font-size:.9rem;
  line-height:1.85;
  color:rgba(255,255,255,.75);
  margin-bottom:1.2em;
}
.bp-text p strong{color:var(--cyan)}
.terminal-block{
  background:#060a0e;
  border:1px solid rgba(0,229,255,.2);
  padding:32px;
  font-family:'JetBrains Mono',monospace;
  font-size:.82rem;
  line-height:1.9;
}
.terminal-block .t-comment{color:rgba(0,229,255,.4)}
.terminal-block .t-key{color:var(--cyan)}
.terminal-block .t-val{color:#fff}
.terminal-block .t-num{color:var(--gold)}
.circuit-wrap{margin-top:40px;display:flex;justify-content:center}

/* ── STORY 4: IMPACT — UK Quantum ────────────────────── */
#s4{
  min-height:100vh;
  background:var(--rose);
  color:#fff;
  display:grid;
  grid-template-columns:1fr 1fr;
}
.impact-left{
  padding:80px;
  display:flex;
  flex-direction:column;
  justify-content:space-between;
}
.impact-stamp{
  display:inline-block;
  border:5px solid rgba(255,255,255,.9);
  padding:10px 24px;
  font-family:'Fraunces',serif;
  font-size:2.2rem;
  font-weight:900;
  letter-spacing:.12em;
  transform:rotate(-3deg);
  width:max-content;
  margin-bottom:48px;
  text-transform:uppercase;
}
.impact-hed{
  font-family:'Fraunces',serif;
  font-size:clamp(2.8rem,6vw,5.2rem);
  font-weight:900;
  line-height:.95;
  margin-bottom:40px;
}
.impact-body p{
  font-size:1rem;
  line-height:1.8;
  color:rgba(255,255,255,.85);
  margin-bottom:1.2em;
}
.impact-figure{
  font-family:'Fraunces',serif;
  font-size:4rem;
  font-weight:900;
  color:rgba(255,255,255,.2);
  line-height:1;
  margin-top:auto;
}
.impact-right{
  background:rgba(0,0,0,.2);
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  padding:80px;
  gap:40px;
}
.impact-stat{
  text-align:center;
  padding:32px;
  border:1px solid rgba(255,255,255,.2);
  width:100%;
}
.impact-stat .num{
  font-family:'Fraunces',serif;
  font-size:3.5rem;
  font-weight:900;
  line-height:1;
}
.impact-stat .lbl{
  font-size:.88rem;
  color:rgba(255,255,255,.65);
  margin-top:8px;
  letter-spacing:.06em;
  text-transform:uppercase;
}

/* ── STORY 5: FEATURE — Colorado Corridor ────────────── */
#s5{
  min-height:100vh;
  background:#1e2b1f;
  color:#e8dcc4;
}
.feature-header{
  padding:64px 80px 48px;
  border-bottom:1px solid rgba(232,220,196,.15);
}
.feature-eyebrow{
  font-family:'JetBrains Mono',monospace;
  font-size:.75rem;
  letter-spacing:.28em;
  text-transform:uppercase;
  color:var(--gold);
  margin-bottom:20px;
}
.feature-hed{
  font-family:'Fraunces',serif;
  font-size:clamp(3rem,6.5vw,5.5rem);
  font-weight:900;
  line-height:.95;
  color:#fff;
}
.feature-hed em{font-style:italic;color:var(--gold)}
.feature-body{
  padding:56px 80px 80px;
  display:grid;
  grid-template-columns:1.2fr 1fr;
  gap:72px;
}
.feature-text p{
  font-size:1.05rem;
  line-height:1.8;
  color:#c8bda0;
  margin-bottom:1.3em;
}
.feature-text p:first-child{
  font-size:1.2rem;
  color:#e8dcc4;
  font-weight:300;
}
.feature-sidebar{}
.mountain-wrap{margin-bottom:32px}
.hub-list{list-style:none}
.hub-list li{
  padding:18px 0;
  border-bottom:1px solid rgba(232,220,196,.12);
  font-size:.92rem;
  color:#a09070;
  line-height:1.6;
}
.hub-list li strong{color:#e8dcc4;display:block;font-size:1rem;margin-bottom:4px}

/* ── STORY 6: LAB REPORT — Quantum Sensing ───────────── */
#s6{
  min-height:100vh;
  background:#faf6ee;
  color:#1a140a;
}
.s6-header{
  padding:64px 80px 0;
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:80px;
  align-items:end;
}
.s6-hed{
  font-family:'Fraunces',serif;
  font-size:clamp(2.8rem,6vw,5rem);
  font-weight:900;
  line-height:.95;
}
.s6-intro{
  font-size:1.15rem;
  line-height:1.7;
  color:#5a4a30;
  padding-top:24px;
  border-top:2px solid #1a140a;
}
.s6-divider{
  height:1px;
  background:#d0c4a8;
  margin:48px 80px;
}
.s6-body{
  padding:0 80px 80px;
  display:grid;
  grid-template-columns:1fr 1fr 1fr;
  gap:48px;
}
.s6-card{padding:32px 0;border-top:3px solid #1a140a}
.s6-card h3{
  font-family:'Fraunces',serif;
  font-size:1.6rem;
  font-weight:700;
  margin-bottom:16px;
  line-height:1.2;
}
.s6-card p{font-size:.95rem;line-height:1.8;color:#4a3a22}
.sensing-wrap{display:flex;justify-content:center;padding:40px 80px 0;grid-column:1/-1}

/* ── STORY 7: BLUEPRINT — EU Quantum ─────────────────── */
#s7{
  min-height:100vh;
  background:#050e08;
  color:var(--jade);
  background-image:
    linear-gradient(rgba(0,184,134,.05) 1px,transparent 1px),
    linear-gradient(90deg,rgba(0,184,134,.05) 1px,transparent 1px);
  background-size:60px 60px;
}
.s7-header{
  padding:64px 80px 40px;
  border-bottom:1px solid rgba(0,184,134,.2);
}
.s7-tag{
  font-family:'JetBrains Mono',monospace;
  font-size:.72rem;
  letter-spacing:.28em;
  text-transform:uppercase;
  padding:5px 14px;
  border:1px solid var(--jade);
  display:inline-block;
  margin-bottom:24px;
}
.s7-hed{
  font-family:'Fraunces',serif;
  font-size:clamp(2.5rem,6vw,5rem);
  font-weight:900;
  line-height:.95;
  color:#fff;
}
.s7-hed span{font-style:italic;color:var(--jade)}
.s7-body{
  padding:56px 80px 80px;
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:64px;
}
.s7-text p{
  font-family:'JetBrains Mono',monospace;
  font-size:.88rem;
  line-height:1.9;
  color:rgba(255,255,255,.7);
  margin-bottom:1.2em;
}
.s7-text p strong{color:var(--jade)}
.s7-milestones{display:flex;flex-direction:column;gap:20px}
.milestone{
  background:rgba(0,184,134,.05);
  border:1px solid rgba(0,184,134,.15);
  padding:24px 28px;
  font-family:'JetBrains Mono',monospace;
}
.milestone .m-year{color:var(--jade);font-size:.72rem;letter-spacing:.2em;margin-bottom:8px;display:block}
.milestone .m-text{color:rgba(255,255,255,.75);font-size:.82rem;line-height:1.65}
.eu-wrap{display:flex;justify-content:center;align-items:center;padding-top:24px}

/* ── STORY 8: PROFILE — Category Architects ──────────── */
#s8{
  min-height:100vh;
  background:#f0ead6;
  color:#2c1810;
}
.profile-header{
  padding:80px 80px 0;
  text-align:center;
  border-bottom:1px solid #d4c4a0;
  padding-bottom:48px;
}
.profile-rubric{
  font-family:'JetBrains Mono',monospace;
  font-size:.72rem;
  letter-spacing:.3em;
  text-transform:uppercase;
  color:#8a6a40;
  margin-bottom:24px;
  display:block;
}
.profile-hed{
  font-family:'Fraunces',serif;
  font-size:clamp(3rem,7vw,5.8rem);
  font-weight:900;
  font-style:italic;
  line-height:.95;
  color:#2c1810;
}
.profile-sub{
  font-size:1.1rem;
  color:#7a5a38;
  margin-top:20px;
  max-width:640px;
  margin-left:auto;
  margin-right:auto;
}
.profiles-grid{
  padding:64px 80px 80px;
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:64px;
}
.profile-card{padding-top:40px;border-top:3px solid #2c1810}
.profile-card .p-name{
  font-family:'Fraunces',serif;
  font-size:2.2rem;
  font-weight:700;
  line-height:1;
  margin-bottom:6px;
}
.profile-card .p-title{
  font-size:.88rem;
  color:#8a6a40;
  letter-spacing:.06em;
  text-transform:uppercase;
  margin-bottom:24px;
  display:block;
}
.profile-card p{
  font-size:.98rem;
  line-height:1.8;
  color:#4a3020;
  margin-bottom:1em;
}

/* ── STORY 9: IMPACT — Japan Photonics ───────────────── */
#s9{
  min-height:100vh;
  background:var(--indigo);
  color:#fff;
}
.s9-header{
  padding:72px 80px 48px;
  border-bottom:1px solid rgba(255,255,255,.1);
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:80px;
  align-items:center;
}
.s9-stamp{
  display:inline-block;
  border:4px solid var(--gold);
  padding:8px 20px;
  font-family:'Fraunces',serif;
  font-size:1.8rem;
  font-weight:900;
  letter-spacing:.1em;
  color:var(--gold);
  transform:rotate(-2deg);
  width:max-content;
  margin-bottom:32px;
  text-transform:uppercase;
}
.s9-hed{
  font-family:'Fraunces',serif;
  font-size:clamp(2.5rem,6vw,4.8rem);
  font-weight:900;
  line-height:.95;
}
.s9-hed span{font-style:italic;color:var(--gold)}
.s9-intro{
  font-size:1.1rem;
  color:rgba(255,255,255,.7);
  line-height:1.75;
}
.s9-body{
  padding:56px 80px 80px;
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:64px;
}
.s9-body p{
  font-size:1rem;
  line-height:1.8;
  color:rgba(255,255,255,.75);
  margin-bottom:1.2em;
}
.s9-specs{display:flex;flex-direction:column;gap:16px}
.s9-spec{
  display:flex;
  justify-content:space-between;
  align-items:baseline;
  padding:18px 0;
  border-bottom:1px solid rgba(255,255,255,.1);
}
.s9-spec .sp-label{font-size:.82rem;color:rgba(255,255,255,.5);letter-spacing:.06em;text-transform:uppercase}
.s9-spec .sp-val{
  font-family:'Fraunces',serif;
  font-size:1.8rem;
  font-weight:700;
  color:var(--gold);
}
.photon-wrap{display:flex;justify-content:center;padding:0 80px 40px}

/* ── STORY 10: FEATURE — Quantum Network ─────────────── */
#s10{
  min-height:100vh;
  background:#040c16;
  color:#c8dff0;
}
.s10-header{
  padding:72px 80px 48px;
  border-bottom:1px solid rgba(200,223,240,.08);
}
.s10-eyebrow{
  font-family:'JetBrains Mono',monospace;
  font-size:.75rem;
  letter-spacing:.28em;
  text-transform:uppercase;
  color:var(--electric);
  margin-bottom:20px;
  display:block;
}
.s10-hed{
  font-family:'Fraunces',serif;
  font-size:clamp(3rem,7vw,6rem);
  font-weight:900;
  line-height:.9;
  color:#fff;
}
.s10-hed em{font-style:italic;color:var(--electric)}
.s10-body{
  padding:56px 80px 80px;
  display:grid;
  grid-template-columns:1.4fr 1fr;
  gap:72px;
  align-items:start;
}
.s10-text p{
  font-size:1.05rem;
  line-height:1.8;
  color:#99b8cc;
  margin-bottom:1.3em;
}
.s10-text p:first-child{color:#c8dff0;font-size:1.18rem}
.s10-pullquote{
  font-family:'Fraunces',serif;
  font-size:1.6rem;
  font-weight:300;
  font-style:italic;
  color:var(--electric);
  line-height:1.4;
  padding:32px 0;
  border-top:1px solid rgba(200,223,240,.15);
  border-bottom:1px solid rgba(200,223,240,.15);
  margin:32px 0;
}
.network-wrap{display:flex;justify-content:center;align-items:center;height:340px}

/* ── STORY 11: CLOSING HERO ──────────────────────────── */
#s11{
  min-height:100vh;
  background:#000;
  color:#fff;
  display:flex;
  flex-direction:column;
  justify-content:center;
  padding:80px;
  position:relative;
}
.s11-hed{
  font-family:'Fraunces',serif;
  font-size:clamp(4rem,11vw,9.5rem);
  font-weight:900;
  font-style:italic;
  line-height:.88;
  max-width:1100px;
  margin-bottom:64px;
}
.s11-hed span{display:block;color:var(--electric);font-style:normal}
.s11-manifesto{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:48px;
  max-width:1100px;
  border-top:1px solid #222;
  padding-top:48px;
}
.manifesto-p{
  font-size:1rem;
  line-height:1.8;
  color:#888;
}
.manifesto-p strong{color:#fff}
.s11-closer{
  margin-top:64px;
  display:flex;
  align-items:center;
  gap:24px;
  padding-top:40px;
  border-top:1px solid #111;
}
.s11-wordmark{
  font-family:'Fraunces',serif;
  font-size:1.1rem;
  font-weight:700;
  letter-spacing:.05em;
  color:#fff;
}
.s11-date{
  font-family:'JetBrains Mono',monospace;
  font-size:.72rem;
  color:#555;
  letter-spacing:.15em;
  text-transform:uppercase;
}
@keyframes dawn-pulse{0%,100%{opacity:.3}50%{opacity:.7}}
.dawn-line{animation:dawn-pulse 4s ease-in-out infinite}

/* ── FOOTER ──────────────────────────────────────────── */
footer{
  background:#060606;
  border-top:1px solid #181818;
  padding:56px 80px;
  display:grid;
  grid-template-columns:1fr 1fr 1fr;
  gap:48px;
}
.foot-col h4{
  font-family:'JetBrains Mono',monospace;
  font-size:.72rem;
  letter-spacing:.25em;
  text-transform:uppercase;
  color:var(--electric);
  margin-bottom:20px;
}
.foot-col p,.foot-col ul{
  font-size:.88rem;
  color:#555;
  line-height:1.75;
}
.foot-col ul{list-style:none}
.foot-col ul li{padding:4px 0;border-bottom:1px solid #111}
.foot-col ul li span{color:#888}

</style>
</head>
<body>

<!-- ══════════════════════════════════════════════════════
     COVER
═══════════════════════════════════════════════════════ -->
<section id="cover">
  <div class="cover-left">
    <span class="issue-tag">Special Edition · World Quantum Day · April 14, 2026</span>
    <h1 class="cover-title">The <em>Quantum</em> Record</h1>
    <p class="cover-sub">Eleven dispatches from the frontier — commercial milestones, regional ecosystems, the humans building the field, and the weird science rewriting what "useful" means.</p>
    <span class="cover-dateline">Vol. I — April 14, 2026 — π × 10⁷</span>
  </div>
  <div class="cover-right">
    <!-- Bloch Sphere SVG -->
    <svg viewBox="0 0 400 400" width="400" height="400" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <radialGradient id="sph-grad" cx="42%" cy="38%">
          <stop offset="0%" stop-color="#1a2a40"/>
          <stop offset="100%" stop-color="#050810"/>
        </radialGradient>
        <filter id="glow"><feGaussianBlur stdDeviation="3" result="blur"/><feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge></filter>
      </defs>
      <!-- Sphere body -->
      <circle cx="200" cy="200" r="160" fill="url(#sph-grad)" stroke="#1a3050" stroke-width="1"/>
      <!-- Equator ellipse -->
      <ellipse cx="200" cy="200" rx="160" ry="44" fill="none" stroke="rgba(43,170,255,.2)" stroke-width="1" stroke-dasharray="4 4"/>
      <!-- Vertical circle -->
      <ellipse cx="200" cy="200" rx="44" ry="160" fill="none" stroke="rgba(43,170,255,.15)" stroke-width="1" stroke-dasharray="4 4"/>
      <!-- Z-axis -->
      <line x1="200" y1="28" x2="200" y2="372" stroke="rgba(43,170,255,.3)" stroke-width="1"/>
      <!-- X-axis -->
      <line x1="40" y1="200" x2="360" y2="200" stroke="rgba(43,170,255,.3)" stroke-width="1"/>
      <!-- Orbit rings (animated) -->
      <g class="orbit1">
        <ellipse cx="200" cy="200" rx="130" ry="36" fill="none" stroke="rgba(43,170,255,.35)" stroke-width="1.2"/>
        <circle cx="330" cy="200" r="5" fill="#2BAAFF" filter="url(#glow)" class="state-dot"/>
      </g>
      <g class="orbit2">
        <ellipse cx="200" cy="200" rx="90" ry="90" fill="none" stroke="rgba(0,229,255,.2)" stroke-width="1" transform="rotate(30 200 200)"/>
        <circle cx="200" cy="110" r="4" fill="#00E5FF" filter="url(#glow)" class="state-dot-2"/>
      </g>
      <g class="orbit3">
        <ellipse cx="200" cy="200" rx="155" ry="42" fill="none" stroke="rgba(201,169,75,.25)" stroke-width="1" transform="rotate(-20 200 200)"/>
      </g>
      <!-- State vector -->
      <line x1="200" y1="200" x2="280" y2="118" stroke="#fff" stroke-width="2" filter="url(#glow)"/>
      <circle cx="280" cy="118" r="6" fill="#fff" filter="url(#glow)"/>
      <!-- Poles -->
      <text x="208" y="24" font-family="JetBrains Mono,monospace" font-size="12" fill="rgba(43,170,255,.7)">|0⟩</text>
      <text x="208" y="388" font-family="JetBrains Mono,monospace" font-size="12" fill="rgba(43,170,255,.7)">|1⟩</text>
      <text x="348" y="204" font-family="JetBrains Mono,monospace" font-size="11" fill="rgba(43,170,255,.5)">x</text>
      <!-- Label -->
      <text x="200" y="440" text-anchor="middle" font-family="JetBrains Mono,monospace" font-size="11" fill="rgba(255,255,255,.2)" letter-spacing="4">BLOCH SPHERE</text>
    </svg>
  </div>
</section>

<!-- Table of Contents -->
<nav id="toc">
  <a class="toc-entry" href="#s1"><span class="toc-n">01</span>The Logical Qubit Moment</a>
  <a class="toc-entry" href="#s2"><span class="toc-n">02</span>Microsoft's Topological Gambit</a>
  <a class="toc-entry" href="#s3"><span class="toc-n">03</span>Willow's Warning Shot</a>
  <a class="toc-entry" href="#s4"><span class="toc-n">04</span>Britain Doubles Down</a>
  <a class="toc-entry" href="#s5"><span class="toc-n">05</span>The Mile-High Corridor</a>
  <a class="toc-entry" href="#s6"><span class="toc-n">06</span>Sensing the Unsensable</a>
  <a class="toc-entry" href="#s7"><span class="toc-n">07</span>Europe's Quantum Decade</a>
  <a class="toc-entry" href="#s8"><span class="toc-n">08</span>Neutral-Atom Expansion</a>
  <a class="toc-entry" href="#s9"><span class="toc-n">09</span>Japan Goes Photonic</a>
  <a class="toc-entry" href="#s10"><span class="toc-n">10</span>The Quantum Internet</a>
  <a class="toc-entry" href="#s11"><span class="toc-n">11</span>The Useful Quantum Era</a>
</nav>

<!-- ══════════════════════════════════════════════════════
     STORY 01 · HERO · QuEra & the Logical Qubit
═══════════════════════════════════════════════════════ -->
<section id="s1">
  <div class="s1-top">
    <span class="story-tag">Commercial Milestone</span>
    <span style="font-family:'JetBrains Mono',monospace;font-size:.72rem;color:#666;letter-spacing:.15em">Story 01 of 11</span>
  </div>
  <div class="s1-body">
    <h2 class="s1-hed">
      <span class="kicker">The moment everything changes —</span>
      The Logical<br>Qubit<br><span style="color:var(--electric);font-style:italic">Has Arrived.</span>
    </h2>
    <div>
      <p class="s1-dek">In a December 2023 <em>Nature</em> paper, a team spanning QuEra Computing, Harvard, MIT, and NIST-UMD demonstrated 48 logical qubits with error rates that outperformed physical qubits in key regimes — a significant landmark for the neutral-atom platform and for quantum error correction at scale.</p>
      <div class="s1-body-text">
        <p>For most of quantum computing's history, every qubit added to a system also added noise. The machines grew louder as they grew larger — a cruel physics tax that seemed to make scale impossible. Then, in a series of experiments that compressed a decade of theoretical progress into a single publication cycle, QuEra's team showed that careful engineering of atomic arrays could invert that relationship entirely.</p>
        <p>The key insight was architectural. By arranging rubidium atoms in reconfigurable optical tweezers and applying quantum error correction at the hardware level, the team demonstrated logical error rates that outperformed physical qubits in certain regimes — a relationship that had previously run in the other direction. Larger arrays were, in those regimes, performing better than smaller ones.</p>
        <p>A logical qubit is not merely a better physical qubit — it is a different kind of computing primitive, one that can be wired into algorithms that require error-corrected operations. The experiment demonstrated this at a scale the field had not previously achieved, and set a benchmark for what neutral-atom platforms can deliver when error correction is applied systematically.</p>
      </div>
    </div>
    <div>
      <div class="stat-card">
        <div class="stat-num">48</div>
        <div class="stat-unit">logical qubits</div>
        <div class="stat-desc">Published in <em>Nature</em>, December 6, 2023 (QuEra, Harvard, MIT, NIST-UMD) — showing logical error rates outperforming physical qubits in key regimes, the largest such demonstration on a neutral-atom platform to date.</div>
      </div>
      <div class="lattice-wrap">
        <!-- Neutral Atom Lattice SVG -->
        <svg viewBox="0 0 340 240" width="340" height="240" xmlns="http://www.w3.org/2000/svg">
          <defs>
            <filter id="atom-glow"><feGaussianBlur stdDeviation="2.5" result="b"/><feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge></filter>
          </defs>
          <rect width="340" height="240" fill="#0a0a0a"/>
          <!-- Grid lines -->
          <g stroke="rgba(43,170,255,.06)" stroke-width="1">
            <line x1="0" y1="40" x2="340" y2="40"/><line x1="0" y1="80" x2="340" y2="80"/>
            <line x1="0" y1="120" x2="340" y2="120"/><line x1="0" y1="160" x2="340" y2="160"/>
            <line x1="0" y1="200" x2="340" y2="200"/>
            <line x1="40" y1="0" x2="40" y2="240"/><line x1="80" y1="0" x2="80" y2="240"/>
            <line x1="120" y1="0" x2="120" y2="240"/><line x1="160" y1="0" x2="160" y2="240"/>
            <line x1="200" y1="0" x2="200" y2="240"/><line x1="240" y1="0" x2="240" y2="240"/>
            <line x1="280" y1="0" x2="280" y2="240"/>
          </g>
          <!-- Atoms — blue = logical qubit, dim = physical -->
          <g filter="url(#atom-glow)">
            <!-- Row 1 -->
            <circle cx="40" cy="40" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="80" cy="40" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="120" cy="40" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="160" cy="40" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="200" cy="40" r="6" fill="#333" opacity=".8"/>
            <circle cx="240" cy="40" r="6" fill="#333" opacity=".8"/>
            <circle cx="280" cy="40" r="7" fill="#2BAAFF" opacity=".9"/>
            <!-- Row 2 -->
            <circle cx="40" cy="80" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="80" cy="80" r="6" fill="#333" opacity=".8"/>
            <circle cx="120" cy="80" r="7" fill="#00E5FF" opacity=".95"/>
            <circle cx="160" cy="80" r="7" fill="#00E5FF" opacity=".95"/>
            <circle cx="200" cy="80" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="240" cy="80" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="280" cy="80" r="6" fill="#333" opacity=".8"/>
            <!-- Row 3 -->
            <circle cx="40" cy="120" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="80" cy="120" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="120" cy="120" r="6" fill="#333" opacity=".8"/>
            <circle cx="160" cy="120" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="200" cy="120" r="7" fill="#00E5FF" opacity=".95"/>
            <circle cx="240" cy="120" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="280" cy="120" r="7" fill="#2BAAFF" opacity=".9"/>
            <!-- Row 4 -->
            <circle cx="40" cy="160" r="6" fill="#333" opacity=".8"/>
            <circle cx="80" cy="160" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="120" cy="160" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="160" cy="160" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="200" cy="160" r="6" fill="#333" opacity=".8"/>
            <circle cx="240" cy="160" r="7" fill="#00E5FF" opacity=".95"/>
            <circle cx="280" cy="160" r="7" fill="#2BAAFF" opacity=".9"/>
            <!-- Row 5 -->
            <circle cx="40" cy="200" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="80" cy="200" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="120" cy="200" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="160" cy="200" r="6" fill="#333" opacity=".8"/>
            <circle cx="200" cy="200" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="240" cy="200" r="7" fill="#2BAAFF" opacity=".9"/>
            <circle cx="280" cy="200" r="7" fill="#2BAAFF" opacity=".9"/>
          </g>
          <text x="12" y="230" font-family="JetBrains Mono,monospace" font-size="9" fill="rgba(43,170,255,.4)" letter-spacing="2">NEUTRAL ATOM ARRAY · AQUILA PLATFORM</text>
        </svg>
      </div>
    </div>
  </div>
</section>

<!-- ══════════════════════════════════════════════════════
     STORY 02 · LAB REPORT · Microsoft Topological
═══════════════════════════════════════════════════════ -->
<section id="s2">
  <div class="lab-header">
    <h2 class="lab-hed">Microsoft's<br>Topological Gambit</h2>
    <div class="lab-meta">
      <span class="story-tag" style="color:#8B1A1A">Lab Report</span><br>
      Story 02 of 11<br>
      Keywords: Majorana · Anyons · Error Correction
    </div>
  </div>
  <div class="lab-body">
    <div class="lab-col-left">
      <p>The announcement came in February 2025 and the field has been arguing about it ever since. Microsoft's Majorana 1 chip — a slab of indium arsenide sandwiched against aluminum — is claimed to host topological qubits: quantum states protected not by active error correction, but by the braided trajectories of non-Abelian anyons through spacetime itself. If the physics holds, it would mean a qubit that simply cannot be corrupted by local noise, because the information is encoded globally in the topology of the braid.</p>
      <p>The theory dates to Alexei Kitaev's 2003 paper, which outlined how Majorana zero modes at the ends of a one-dimensional wire could store a qubit with exponential protection. Microsoft's bet, now more than a decade and several billion dollars old, has always been that this topological protection would deliver fault tolerance with far fewer physical components than the surface-code approaches pursued by Google, IBM, and QuEra.</p>
      <p>The evidence remains contested. Independent research groups have struggled to reproduce the spectroscopic signatures Microsoft uses as evidence for Majorana modes. But the Majorana 1 chip represents the most concrete hardware manifestation of the topological program to date — and Microsoft's claim that it can demonstrate qubit operations with error rates sufficient for quantum advantage has raised the possibility, however disputed, that the topological path may yet arrive.</p>
    </div>
    <div class="lab-col-right">
      <p class="lab-pullquote">"The braid is the memory. The memory cannot be erased without undoing the braid. That is the entire bet."</p>
      <!-- Topological Braid SVG -->
      <div class="braid-wrap">
        <svg viewBox="0 0 260 180" width="260" height="180" xmlns="http://www.w3.org/2000/svg">
          <defs>
            <filter id="braid-glow"><feGaussianBlur stdDeviation="2" result="b"/><feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge></filter>
          </defs>
          <rect width="260" height="180" fill="#f5edd8"/>
          <!-- Strand A -->
          <path d="M 40,20 C 40,60 100,60 100,100 C 100,140 160,140 160,180" fill="none" stroke="#8B1A1A" stroke-width="4" filter="url(#braid-glow)" opacity=".85"/>
          <!-- Strand B (crosses over A) -->
          <path d="M 130,20 C 130,60 40,60 40,100" fill="none" stroke="#f5edd8" stroke-width="7"/>
          <path d="M 130,20 C 130,60 40,60 40,100" fill="none" stroke="#5a3e2b" stroke-width="3.5" filter="url(#braid-glow)" opacity=".85"/>
          <path d="M 40,100 C 40,140 130,140 130,180" fill="none" stroke="#5a3e2b" stroke-width="3.5" filter="url(#braid-glow)" opacity=".85"/>
          <!-- Strand C -->
          <path d="M 220,20 C 220,60 160,60 160,100 C 160,140 220,140 220,180" fill="none" stroke="#1a4a2a" stroke-width="4" filter="url(#braid-glow)" opacity=".8"/>
          <!-- Anyon dots -->
          <circle cx="40" cy="20" r="7" fill="#8B1A1A" filter="url(#braid-glow)"/>
          <circle cx="130" cy="20" r="7" fill="#5a3e2b" filter="url(#braid-glow)"/>
          <circle cx="220" cy="20" r="7" fill="#1a4a2a" filter="url(#braid-glow)"/>
          <circle cx="160" cy="180" r="7" fill="#8B1A1A" filter="url(#braid-glow)"/>
          <circle cx="130" cy="180" r="7" fill="#5a3e2b" filter="url(#braid-glow)"/>
          <circle cx="220" cy="180" r="7" fill="#1a4a2a" filter="url(#braid-glow)"/>
          <text x="130" y="170" text-anchor="middle" font-family="JetBrains Mono,monospace" font-size="8.5" fill="#8a7b5c" letter-spacing="2">ANYON WORLD-LINES</text>
        </svg>
      </div>
      <div class="lab-aside">
        <strong>Key Numbers</strong>
        Physical qubit count: classified / Topological protection: T₁ equivalent ~1ms claimed / Independent verification: pending peer review / Investment to date: est. $3B+
      </div>
    </div>
  </div>
</section>

<!-- ══════════════════════════════════════════════════════
     STORY 03 · BLUEPRINT · Google Willow
═══════════════════════════════════════════════════════ -->
<section id="s3">
  <div class="bp-header">
    <span class="bp-tag">Blueprint</span>
    <span class="bp-tagline">// SYSTEM REPORT · ERROR CORRECTION THRESHOLD ANALYSIS · STORY 03</span>
  </div>
  <h2 class="bp-hed">Willow's<br><span>Warning Shot</span></h2>
  <div class="bp-body">
    <div class="bp-text">
      <p>In December 2024, Google published results from its Willow superconducting chip that crossed a line physicists had theorized about for thirty years: <strong>below-threshold quantum error correction at scale</strong>. The chip's error rates decreased as the system grew — the essential prerequisite for any practical quantum computer. Willow completed a standard benchmark computation in under five minutes that would have taken the world's fastest classical supercomputer an estimated 10 septillion years.</p>
      <p>The benchmark is synthetic — designed to be hard for classical machines and easy for quantum ones — but the underlying physics achievement is real. Google demonstrated that a 105-qubit system, using a distance-7 surface code, could perform error-corrected operations with logical error rates below the fault-tolerance threshold. This is the first time any team has demonstrated this at scale without hand-picking favorable conditions.</p>
      <p>The immediate competitive pressure on IBM, QuEra, IonQ, and Microsoft was palpable. Each company has a different theory of how to reach fault tolerance; Willow confirmed that at least one of those theories is close to working at the hardware level. The race is no longer about whether fault tolerance is achievable — it's about who gets there first at useful qubit counts.</p>
    </div>
    <div>
      <div class="terminal-block">
        <div class="t-comment">// WILLOW CHIP · PERFORMANCE SUMMARY</div>
        <div class="t-comment">// December 2024 · Google Quantum AI</div>
        <br>
        <div><span class="t-key">chip.name</span>            <span class="t-val">= "Willow"</span></div>
        <div><span class="t-key">physical_qubits</span>      <span class="t-num">= 105</span></div>
        <div><span class="t-key">error_code</span>           <span class="t-val">= "surface_code"</span></div>
        <div><span class="t-key">code_distance</span>        <span class="t-num">= 7</span></div>
        <div><span class="t-key">threshold_crossed</span>    <span class="t-val">= true  ✓</span></div>
        <br>
        <div><span class="t-key">benchmark_task</span>       <span class="t-val">= "RCS"</span></div>
        <div><span class="t-key">quantum_time</span>         <span class="t-num">= "< 5 min"</span></div>
        <div><span class="t-key">classical_equiv</span>      <span class="t-val">= "10^25 years"</span></div>
        <br>
        <div class="t-comment">// ERROR SCALING (distance d)</div>
        <div><span class="t-key">d3_logical_err</span>       <span class="t-num">= 0.0082</span></div>
        <div><span class="t-key">d5_logical_err</span>       <span class="t-num">= 0.0041</span></div>
        <div><span class="t-key">d7_logical_err</span>       <span class="t-num">= 0.0022</span></div>
        <div class="t-comment">// ↑ Error halves with each code distance step</div>
        <br>
        <div><span class="t-key">status</span>               <span class="t-val">= "THRESHOLD CROSSED"</span></div>
      </div>
      <!-- Circuit SVG -->
      <div class="circuit-wrap" style="margin-top:32px">
        <svg viewBox="0 0 300 160" width="300" height="160" xmlns="http://www.w3.org/2000/svg">
          <rect width="300" height="160" fill="#060a0e"/>
          <!-- Qubit lines -->
          <g stroke="rgba(0,229,255,.25)" stroke-width="1.2">
            <line x1="10" y1="40" x2="290" y2="40"/>
            <line x1="10" y1="80" x2="290" y2="80"/>
            <line x1="10" y1="120" x2="290" y2="120"/>
          </g>
          <!-- Labels -->
          <text x="8" y="36" font-family="JetBrains Mono,monospace" font-size="9" fill="rgba(0,229,255,.4)">q₀</text>
          <text x="8" y="76" font-family="JetBrains Mono,monospace" font-size="9" fill="rgba(0,229,255,.4)">q₁</text>
          <text x="8" y="116" font-family="JetBrains Mono,monospace" font-size="9" fill="rgba(0,229,255,.4)">q₂</text>
          <!-- H gates -->
          <rect x="44" y="30" width="22" height="20" fill="#060a0e" stroke="#00E5FF" stroke-width="1.2" rx="2"/>
          <text x="55" y="44" text-anchor="middle" font-family="JetBrains Mono,monospace" font-size="10" fill="#00E5FF">H</text>
          <rect x="44" y="70" width="22" height="20" fill="#060a0e" stroke="#00E5FF" stroke-width="1.2" rx="2"/>
          <text x="55" y="84" text-anchor="middle" font-family="JetBrains Mono,monospace" font-size="10" fill="#00E5FF">H</text>
          <!-- CNOT gate q0→q1 -->
          <line x1="100" y1="40" x2="100" y2="80" stroke="#C9A94B" stroke-width="1.5"/>
          <circle cx="100" cy="40" r="4" fill="#C9A94B"/>
          <circle cx="100" cy="80" r="8" fill="none" stroke="#C9A94B" stroke-width="1.5"/>
          <line x1="100" y1="72" x2="100" y2="88" stroke="#C9A94B" stroke-width="1.5"/>
          <line x1="92" y1="80" x2="108" y2="80" stroke="#C9A94B" stroke-width="1.5"/>
          <!-- T gate -->
          <rect x="144" y="30" width="22" height="20" fill="#060a0e" stroke="#00E5FF" stroke-width="1.2" rx="2"/>
          <text x="155" y="44" text-anchor="middle" font-family="JetBrains Mono,monospace" font-size="10" fill="#00E5FF">T</text>
          <!-- CNOT gate q1→q2 -->
          <line x1="190" y1="80" x2="190" y2="120" stroke="#C9A94B" stroke-width="1.5"/>
          <circle cx="190" cy="80" r="4" fill="#C9A94B"/>
          <circle cx="190" cy="120" r="8" fill="none" stroke="#C9A94B" stroke-width="1.5"/>
          <line x1="190" y1="112" x2="190" y2="128" stroke="#C9A94B" stroke-width="1.5"/>
          <line x1="182" y1="120" x2="198" y2="120" stroke="#C9A94B" stroke-width="1.5"/>
          <!-- Measurement -->
          <rect x="248" y="30" width="26" height="20" fill="#060a0e" stroke="rgba(0,229,255,.5)" stroke-width="1" rx="2"/>
          <path d="M 254,48 L 261,37 L 268,48" fill="none" stroke="#00E5FF" stroke-width="1.2"/>
          <line x1="261" y1="37" x2="261" y2="50" stroke="#00E5FF" stroke-width="1.2"/>
          <rect x="248" y="70" width="26" height="20" fill="#060a0e" stroke="rgba(0,229,255,.5)" stroke-width="1" rx="2"/>
          <path d="M 254,88 L 261,77 L 268,88" fill="none" stroke="#00E5FF" stroke-width="1.2"/>
          <line x1="261" y1="77" x2="261" y2="90" stroke="#00E5FF" stroke-width="1.2"/>
          <text x="150" y="152" text-anchor="middle" font-family="JetBrains Mono,monospace" font-size="8.5" fill="rgba(0,229,255,.3)" letter-spacing="2">SURFACE CODE CIRCUIT FRAGMENT</text>
        </svg>
      </div>
    </div>
  </div>
</section>

<!-- ══════════════════════════════════════════════════════
     STORY 04 · IMPACT · UK Quantum
═══════════════════════════════════════════════════════ -->
<section id="s4">
  <div class="impact-left">
    <div>
      <div class="impact-stamp">Impact</div>
      <h2 class="impact-hed">Britain<br>Doubles<br>Down</h2>
    </div>
    <div class="impact-body">
      <p>The UK National Quantum Computing Centre opened its doors at the Harwell Science Campus in 2024, becoming Europe's most significant state-backed quantum computing facility. With £2.5 billion committed to the National Quantum Strategy and a government mandate to position Britain as a top-three global quantum nation, the NQCC is now actively brokering access for pharmaceutical, financial, and defense-sector users.</p>
      <p>What makes the NQCC distinct from similar national programs in Germany and France is its deliberate commercial orientation. Rather than operating as a pure research facility, the centre is structured to allow industrial users to run proprietary workloads on quantum hardware without exposing their algorithms — a privacy architecture that has attracted significant interest from the City of London's financial institutions.</p>
      <p>The UK's ecosystem extends beyond Harwell. Oxford Ionics, Quantum Motion, and Universal Quantum have all closed significant funding rounds since 2024, while Innovate UK has directed £120M in additional quantum grant funding toward industry-ready applications in sensing and communication.</p>
    </div>
    <div class="impact-figure" style="font-size:1.2rem;color:rgba(255,255,255,.5);font-family:'JetBrains Mono',monospace;letter-spacing:.08em">STORY 04 / 11 · REGIONAL ECOSYSTEM</div>
  </div>
  <div class="impact-right">
    <!-- Union Jack Quantum Geometry SVG -->
    <svg viewBox="0 0 300 300" width="280" height="280" xmlns="http://www.w3.org/2000/svg" style="margin-bottom:32px">
      <defs>
        <filter id="uk-glow"><feGaussianBlur stdDeviation="3" result="b"/><feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge></filter>
      </defs>
      <!-- Background -->
      <rect width="300" height="300" fill="rgba(0,0,0,.3)"/>
      <!-- Geometric qubit lattice evoking Union Jack -->
      <g stroke="rgba(255,255,255,.15)" stroke-width="1" fill="none">
        <line x1="0" y1="150" x2="300" y2="150"/>
        <line x1="150" y1="0" x2="150" y2="300"/>
        <line x1="0" y1="0" x2="300" y2="300"/>
        <line x1="300" y1="0" x2="0" y2="300"/>
      </g>
      <!-- Qubit nodes at intersections -->
      <g filter="url(#uk-glow)">
        <circle cx="150" cy="150" r="12" fill="#fff"/>
        <circle cx="150" cy="60" r="7" fill="rgba(255,255,255,.7)"/>
        <circle cx="150" cy="240" r="7" fill="rgba(255,255,255,.7)"/>
        <circle cx="60" cy="150" r="7" fill="rgba(255,255,255,.7)"/>
        <circle cx="240" cy="150" r="7" fill="rgba(255,255,255,.7)"/>
        <circle cx="75" cy="75" r="6" fill="rgba(255,255,255,.5)"/>
        <circle cx="225" cy="75" r="6" fill="rgba(255,255,255,.5)"/>
        <circle cx="75" cy="225" r="6" fill="rgba(255,255,255,.5)"/>
        <circle cx="225" cy="225" r="6" fill="rgba(255,255,255,.5)"/>
        <!-- Entanglement links -->
        <line x1="150" y1="150" x2="150" y2="60" stroke="rgba(255,255,255,.4)" stroke-width="1.5"/>
        <line x1="150" y1="150" x2="150" y2="240" stroke="rgba(255,255,255,.4)" stroke-width="1.5"/>
        <line x1="150" y1="150" x2="60" y2="150" stroke="rgba(255,255,255,.4)" stroke-width="1.5"/>
        <line x1="150" y1="150" x2="240" y2="150" stroke="rgba(255,255,255,.4)" stroke-width="1.5"/>
        <line x1="150" y1="150" x2="75" y2="75" stroke="rgba(255,255,255,.25)" stroke-width="1.2"/>
        <line x1="150" y1="150" x2="225" y2="75" stroke="rgba(255,255,255,.25)" stroke-width="1.2"/>
        <line x1="150" y1="150" x2="75" y2="225" stroke="rgba(255,255,255,.25)" stroke-width="1.2"/>
        <line x1="150" y1="150" x2="225" y2="225" stroke="rgba(255,255,255,.25)" stroke-width="1.2"/>
      </g>
      <text x="150" y="295" text-anchor="middle" font-family="JetBrains Mono,monospace" font-size="9" fill="rgba(255,255,255,.3)" letter-spacing="3">NQCC · HARWELL · OXFORDSHIRE</text>
    </svg>
    <div class="impact-stat"><div class="num">£2.5B</div><div class="lbl">National Quantum Strategy Commitment</div></div>
    <div class="impact-stat"><div class="num">Top 3</div><div class="lbl">Government Target — Global Quantum Nations</div></div>
    <div class="impact-stat"><div class="num">£120M</div><div class="lbl">Innovate UK Applied Quantum Grants</div></div>
  </div>
</section>

<!-- ══════════════════════════════════════════════════════
     STORY 05 · FEATURE · Colorado Corridor
═══════════════════════════════════════════════════════ -->
<section id="s5">
  <div class="feature-header">
    <div class="feature-eyebrow">Regional Ecosystem · Story 05 of 11</div>
    <h2 class="feature-hed">The Mile-High<br><em>Quantum Corridor</em></h2>
  </div>
  <div class="feature-body">
    <div class="feature-text">
      <p>Something is happening in the mountain states. In a geographic arc stretching from Boulder to Albuquerque, a density of quantum talent is forming that rivals any coastline cluster — and doing so without the venture-capital noise that surrounds Boston and the Bay Area.</p>
      <p>The anchor is NIST's JILA laboratory in Boulder, where atomic clock science has been generating quantum technology for half a century. Today JILA spin-outs are becoming companies: precision timing, quantum-enhanced sensors for navigation, optical lattice clocks accurate enough to detect gravitational gradients. The University of Colorado Boulder's quantum engineering program now places graduates directly into QuEra, Vescent, Infleqtion, and a rotating cast of new ventures.</p>
      <p>Forty miles south, the Air Force Research Laboratory at Kirtland Air Force Base is funding quantum sensing programs that don't appear in any press release. Sandia National Laboratories runs the largest government quantum computing program outside of the East Coast. Los Alamos National Lab has a dedicated Quantum Science Center. The Mountain West's quantum ecosystem is, in large part, classified — but its commercial spillover is measurable. The density of talent within a twenty-mile radius of Boulder is, by most accounts, without parallel in the inland United States.</p>
    </div>
    <div class="feature-sidebar">
      <!-- Mountain SVG -->
      <div class="mountain-wrap">
        <svg viewBox="0 0 300 160" width="300" height="160" xmlns="http://www.w3.org/2000/svg">
          <rect width="300" height="160" fill="#1e2b1f"/>
          <!-- Mountain silhouettes -->
          <polygon points="0,160 80,40 140,100 180,55 240,90 300,30 300,160" fill="#162018"/>
          <polygon points="0,160 60,70 120,110 160,65 220,95 280,45 300,60 300,160" fill="#1a2619"/>
          <!-- Snow caps -->
          <polygon points="80,40 65,72 95,72" fill="rgba(232,220,196,.15)"/>
          <polygon points="180,55 168,78 192,78" fill="rgba(232,220,196,.15)"/>
          <polygon points="300,30 288,55 312,55" fill="rgba(232,220,196,.1)"/>
          <!-- Quantum dots in sky -->
          <circle cx="40" cy="25" r="2.5" fill="rgba(201,169,75,.6)"/>
          <circle cx="120" cy="18" r="2" fill="rgba(43,170,255,.5)"/>
          <circle cx="200" cy="22" r="2.5" fill="rgba(201,169,75,.5)"/>
          <circle cx="260" cy="14" r="2" fill="rgba(43,170,255,.4)"/>
          <!-- Connecting lines -->
          <line x1="40" y1="25" x2="120" y2="18" stroke="rgba(201,169,75,.2)" stroke-width="1"/>
          <line x1="120" y1="18" x2="200" y2="22" stroke="rgba(201,169,75,.2)" stroke-width="1"/>
          <line x1="200" y1="22" x2="260" y2="14" stroke="rgba(201,169,75,.2)" stroke-width="1"/>
          <text x="150" y="150" text-anchor="middle" font-family="JetBrains Mono,monospace" font-size="8.5" fill="rgba(201,169,75,.35)" letter-spacing="3">BOULDER · KIRTLAND · SANTA FE</text>
        </svg>
      </div>
      <ul class="hub-list">
        <li><strong>JILA / CU Boulder</strong>Atomic clock spin-outs; optical lattice clocks; quantum sensing foundational research. 70+ quantum-active faculty.</li>
        <li><strong>Sandia National Labs</strong>Largest government QC program in the region. Trapped-ion platforms, quantum networking R&D.</li>
        <li><strong>Los Alamos Quantum Science Center</strong>DOE flagship center. Materials, algorithms, error mitigation across platforms.</li>
        <li><strong>AFRL Kirtland</strong>Classified sensing programs. Quantum PNT (Positioning, Navigation, Timing) at scale.</li>
      </ul>
    </div>
  </div>
</section>

<!-- ══════════════════════════════════════════════════════
     STORY 06 · LAB REPORT · Quantum Sensing
═══════════════════════════════════════════════════════ -->
<section id="s6">
  <div class="s6-header">
    <h2 class="s6-hed">Sensing<br>the<br>Unsensable</h2>
    <p class="s6-intro">The most commercially ready branch of quantum technology isn't a computer. It's a sensor. Quantum gravimeters, magnetometers, and clocks are already deployed in the field — and they're finding things classical instruments cannot.</p>
  </div>
  <hr class="s6-divider">
  <!-- Sensing interference SVG -->
  <div style="display:flex;justify-content:center;padding:0 80px 40px">
    <svg viewBox="0 0 420 180" width="420" height="180" xmlns="http://www.w3.org/2000/svg">
      <rect width="420" height="180" fill="#faf6ee"/>
      <!-- Interference rings -->
      <g fill="none" stroke="#1a140a" stroke-width="1" opacity=".08">
        <circle cx="210" cy="90" r="20"/><circle cx="210" cy="90" r="35"/>
        <circle cx="210" cy="90" r="50"/><circle cx="210" cy="90" r="65"/>
        <circle cx="210" cy="90" r="80"/><circle cx="210" cy="90" r="95"/>
        <circle cx="210" cy="90" r="110"/><circle cx="210" cy="90" r="125"/>
        <circle cx="210" cy="90" r="140"/><circle cx="210" cy="90" r="160"/>
      </g>
      <!-- Atom at center -->
      <circle cx="210" cy="90" r="8" fill="#1a140a"/>
      <circle cx="210" cy="90" r="18" fill="none" stroke="#1a140a" stroke-width="1.5" opacity=".4"/>
      <circle cx="210" cy="90" r="28" fill="none" stroke="#8B1A1A" stroke-width="1" opacity=".35"/>
      <!-- Electron-like marker -->
      <circle cx="228" cy="78" r="3.5" fill="#8B1A1A"/>
      <!-- Wave lines emanating left and right -->
      <path d="M 0,90 Q 30,70 60,90 Q 90,110 120,90 Q 150,70 180,90" fill="none" stroke="#1a140a" stroke-width="1.5" opacity=".18"/>
      <path d="M 240,90 Q 270,70 300,90 Q 330,110 360,90 Q 390,70 420,90" fill="none" stroke="#1a140a" stroke-width="1.5" opacity=".18"/>
      <text x="210" y="170" text-anchor="middle" font-family="JetBrains Mono,monospace" font-size="9" fill="rgba(26,20,10,.35)" letter-spacing="3">ATOMIC INTERFERENCE · MATTER-WAVE GRAVIMETRY</text>
    </svg>
  </div>
  <div class="s6-body">
    <div class="s6-card">
      <h3>Gravimetry Without GPS</h3>
      <p>Atom interferometers split a cloud of ultracold atoms along two paths, then recombine them. The resulting interference fringe encodes the gravitational field at the measurement point with extraordinary precision — enough to map underground cavities, pipelines, and archaeological structures without drilling a hole. The UK and France now field portable quantum gravimeters for infrastructure inspection. The US Army has a program to use them for navigation in GPS-denied environments.</p>
    </div>
    <div class="s6-card">
      <h3>Quantum Magnetometers in Medicine</h3>
      <p>Optically pumped magnetometers using nitrogen-vacancy centers in diamond are approaching SQUID sensitivity without requiring cryogenic cooling. The result is a new generation of magnetoencephalography (MEG) devices — brain scanners that can be worn like a helmet rather than operated in a refrigerated room. Clinical trials for detecting early-stage Parkinson's disease are underway in the UK, Germany, and Australia. The quantum advantage is real, measurable, and insurance-reimbursable.</p>
    </div>
    <div class="s6-card">
      <h3>Atomic Clocks Leave the Lab</h3>
      <p>For fifty years, the world's most precise atomic clocks sat in national metrology labs, communicating time to the rest of the world via radio signals. In 2025, optical lattice clocks small enough to fit in a shipping container began operating aboard research vessels and in military installations. The implications cascade: more precise GPS, better synchronization for financial systems, and the ability to detect volcanic activity and groundwater movement from clock readings alone — a gravitational potential signal encoded in time.</p>
    </div>
  </div>
</section>

<!-- ══════════════════════════════════════════════════════
     STORY 07 · BLUEPRINT · EU Quantum Flagship
═══════════════════════════════════════════════════════ -->
<section id="s7">
  <div class="s7-header">
    <span class="s7-tag">Blueprint · Regional Ecosystem</span>
    <h2 class="s7-hed">Europe's<br>Quantum Decade:<br><span>Year Five</span></h2>
  </div>
  <div class="s7-body">
    <div class="s7-text">
      <p>The EU Quantum Flagship launched in 2018 with a €1 billion, ten-year mandate. Five years in, the program has funded more than 5,000 researchers across 140 projects, produced six working quantum computers accessible through the European Quantum Computing & Simulation Infrastructure (EuroQCS), and — critically — begun generating the industrial relationships that will determine whether European quantum technology remains a research program or becomes an economic force.</p>
      <p>The clearest commercial signal has come from <strong>IQM</strong> in Finland, which delivered superconducting systems to Germany's Leibniz Supercomputing Centre and to VTT, Finland's national research institute, while simultaneously closing commercial contracts with financial-services firms in Frankfurt. IQM's 2025 unaudited revenue is reported at least $35 million USD — modest by Silicon Valley standards, significant for European deep tech.</p>
      <p>Germany's €3B national quantum strategy, operating alongside the Flagship, has funded a parallel track of industrial adoption through Fraunhofer institutes. BASF, Volkswagen, and Deutsche Bahn have all published results from quantum algorithm trials — mostly proof-of-concept, but the corporate commitment to quantum R&D budgets is now institutionalized rather than opportunistic.</p>
      <p>The challenges are structural. Europe's strength in quantum physics research has not yet translated into proportional strength in system integration, software tools, or go-to-market capability. The companies best positioned to capture value from European quantum research are still often American. This gap — between excellent physics and commercial execution — is the defining tension of European quantum policy heading into Year Six.</p>
    </div>
    <div>
      <div class="eu-wrap">
        <!-- EU Stars as Qubit Array SVG -->
        <svg viewBox="0 0 240 240" width="240" height="240" xmlns="http://www.w3.org/2000/svg">
          <rect width="240" height="240" fill="rgba(0,0,0,.3)"/>
          <!-- 12 EU stars arranged as qubit nodes -->
          <g fill="none">
            <!-- Stars replaced with quantum dots connected in EU circle pattern -->
            <g fill="rgba(0,184,134,.7)">
              <circle cx="120" cy="28" r="7"/><circle cx="180" cy="48" r="7"/>
              <circle cx="212" cy="108" r="7"/><circle cx="192" cy="172" r="7"/>
              <circle cx="132" cy="208" r="7"/><circle cx="68" cy="200" r="7"/>
              <circle cx="32" cy="148" r="7"/><circle cx="36" cy="80" r="7"/>
              <circle cx="76" cy="34" r="7"/><circle cx="152" cy="24" r="7"/>
              <circle cx="200" cy="76" r="7"/><circle cx="208" cy="140" r="7"/>
            </g>
            <!-- Connecting ring -->
            <circle cx="120" cy="120" r="96" stroke="rgba(0,184,134,.15)" stroke-width="1" stroke-dasharray="4 4"/>
            <!-- Entanglement lines (selected) -->
            <g stroke="rgba(0,184,134,.3)" stroke-width="1">
              <line x1="120" y1="28" x2="180" y2="48"/>
              <line x1="180" y1="48" x2="212" y2="108"/>
              <line x1="212" y1="108" x2="192" y2="172"/>
              <line x1="120" y1="28" x2="120" y2="120"/>
              <line x1="212" y1="108" x2="120" y2="120"/>
              <line x1="32" y1="148" x2="120" y2="120"/>
              <line x1="36" y1="80" x2="120" y2="120"/>
            </g>
            <!-- Central node -->
            <circle cx="120" cy="120" r="10" fill="rgba(0,184,134,.5)"/>
          </g>
          <text x="120" y="236" text-anchor="middle" font-family="JetBrains Mono,monospace" font-size="8.5" fill="rgba(0,184,134,.35)" letter-spacing="2">EU QUANTUM FLAGSHIP · 2018–2028</text>
        </svg>
      </div>
      <div class="s7-milestones">
        <div class="milestone"><span class="m-year">2018 // LAUNCH</span><span class="m-text">€1B Flagship program begins; 20 pilot projects across computing, sensing, networking, simulation</span></div>
        <div class="milestone"><span class="m-year">2021 // SCALE</span><span class="m-text">EuroQCS infrastructure initiative; first European quantum computers accessible to industry</span></div>
        <div class="milestone"><span class="m-year">2023 // INDUSTRY</span><span class="m-text">IQM delivers commercial superconducting systems. German national quantum strategy adds €3B</span></div>
        <div class="milestone"><span class="m-year">2024 // ADOPTION</span><span class="m-text">BASF, VW, Deutsche Bahn publish quantum algorithm results. EuroQCS reaches 6 operational machines</span></div>
        <div class="milestone"><span class="m-year">2025 // GAP</span><span class="m-text">Review: strong physics, lagging commercialization. Year Six policy shifts toward ecosystem, not just research</span></div>
      </div>
    </div>
  </div>
</section>

<!-- ══════════════════════════════════════════════════════
     STORY 08 · BLUEPRINT · Neutral-Atom Expansion
═══════════════════════════════════════════════════════ -->
<section id="s8">
  <div class="bp-header">
    <span class="bp-tag">Blueprint</span>
    <span class="bp-tagline">// PLATFORM REPORT · NEUTRAL-ATOM EXPANSION · STORY 08 OF 11</span>
  </div>
  <h2 class="bp-hed">Neutral-Atom<br><span>Expansion</span></h2>
  <div class="bp-body">
    <div class="bp-text">
      <p>On March 24, 2026, Google announced that its quantum computing research now includes <strong>neutral-atom systems</strong> alongside its existing superconducting platform. Individual atoms are used as qubits. The company stated that neutral-atom technology is being developed in parallel with its superconducting work — a significant signal that the leading superconducting program in the world considers neutral atoms worth pursuing simultaneously.</p>
      <p>Separately, <strong>Oratomic</strong> is developing neutral-atom quantum computers using only light and atoms. The company describes its focus as reaching the ultra-efficient regime of quantum error correction. Its team, as listed on the company's website, includes Dolev Bluvstein, Madelyn Cain, Jackson Ellis, Manuel Endres, Simon Evered (incoming), Andrei Faraon, Hsin-Yuan Huang, Robbie King, Harry Levine, Hannah Manetsch (incoming), Lewis Picard, Nickolas Pilgram, John Preskill, and Qian Xu.</p>
      <p>The convergence is notable: the neutral-atom platform — which uses laser-trapped Rydberg atoms and reconfigurable optical tweezer arrays — is now being pursued simultaneously by Google, QuEra, Oratomic, and Infleqtion. Each company brings a different architectural emphasis, but the underlying physics is the same: atoms are identical, erasure errors can be detected mid-circuit, and the platform supports long-range connectivity without a fixed coupling graph. The field has chosen its second platform.</p>
    </div>
    <div>
      <div class="terminal-block">
        <div class="t-comment">// NEUTRAL-ATOM PLATFORM SNAPSHOT · Q1 2026</div>
        <br>
        <div class="t-comment">// GOOGLE — March 24, 2026</div>
        <div><span class="t-key">platform_addition</span>  <span class="t-val">= "neutral_atom"</span></div>
        <div><span class="t-key">co_platform</span>         <span class="t-val">= "superconducting"</span></div>
        <div><span class="t-key">qubit_type</span>          <span class="t-val">= "individual_atoms"</span></div>
        <div><span class="t-key">status</span>              <span class="t-val">= "research expansion"</span></div>
        <br>
        <div class="t-comment">// ORATOMIC — new entrant</div>
        <div><span class="t-key">technology</span>          <span class="t-val">= "light + atoms"</span></div>
        <div><span class="t-key">target_regime</span>       <span class="t-val">= "ultra_efficient_QEC"</span></div>
        <div><span class="t-key">team_size</span>           <span class="t-num">= 14  // listed on oratomic.com</span></div>
        <br>
        <div class="t-comment">// PLATFORM CONVERGENCE SIGNAL</div>
        <div><span class="t-key">neutral_atom_orgs</span>   <span class="t-val">= ["QuEra","Google","Oratomic","Infleqtion"]</span></div>
        <div><span class="t-key">shared_physics</span>      <span class="t-val">= "Rydberg_atom_arrays"</span></div>
        <div><span class="t-key">key_advantage</span>       <span class="t-val">= "identical_atoms,erasure_detection"</span></div>
      </div>
    </div>
  </div>
</section>

<!-- ══════════════════════════════════════════════════════
     STORY 09 · IMPACT · Japan Photonics
═══════════════════════════════════════════════════════ -->
<section id="s9">
  <div class="s9-header">
    <div>
      <div class="s9-stamp">Impact</div>
      <h2 class="s9-hed">Japan<br>Goes<br><span>Photonic</span></h2>
    </div>
    <p class="s9-intro">Japan's national quantum program includes sustained research in photonic quantum computing through NTT Corporation and the National Institute of Information and Communications Technology (NICT). Photonic qubits are encoded in properties of individual photons and can, in principle, operate at room temperature while interfacing with existing fiber-optic networks.</p>
  </div>
  <!-- Photon wave SVG -->
  <div class="photon-wrap">
    <svg viewBox="0 0 600 100" width="600" height="100" xmlns="http://www.w3.org/2000/svg">
      <rect width="600" height="100" fill="rgba(0,0,0,.3)"/>
      <!-- Wave 1 -->
      <path d="M 0,50 Q 37,10 75,50 Q 113,90 150,50 Q 188,10 225,50 Q 263,90 300,50 Q 338,10 375,50 Q 413,90 450,50 Q 488,10 525,50 Q 563,90 600,50" fill="none" stroke="rgba(201,169,75,.6)" stroke-width="2"/>
      <!-- Wave 2 (offset) -->
      <path d="M 0,50 Q 37,90 75,50 Q 113,10 150,50 Q 188,90 225,50 Q 263,10 300,50 Q 338,90 375,50 Q 413,10 450,50 Q 488,90 525,50 Q 563,10 600,50" fill="none" stroke="rgba(201,169,75,.25)" stroke-width="1.5"/>
      <!-- Photon particles -->
      <circle cx="75" cy="50" r="5" fill="var(--gold)" opacity=".8"/>
      <circle cx="225" cy="50" r="5" fill="var(--gold)" opacity=".8"/>
      <circle cx="375" cy="50" r="5" fill="var(--gold)" opacity=".8"/>
      <circle cx="525" cy="50" r="5" fill="var(--gold)" opacity=".8"/>
      <text x="300" y="92" text-anchor="middle" font-family="JetBrains Mono,monospace" font-size="9" fill="rgba(201,169,75,.3)" letter-spacing="3">PHOTONIC QUBIT · SINGLE-PHOTON INTERFERENCE</text>
    </svg>
  </div>
  <div class="s9-body">
    <div>
      <p>NTT Corporation and NICT have maintained active photonic quantum research programs focused on room-temperature operation and fiber-optic compatibility. Photonic qubits — encoded in the polarization, phase, or path of individual photons — do not require the dilution refrigerators that make superconducting quantum computers expensive to operate and difficult to scale.</p>
      <p>The photonic approach faces its own engineering challenges: deterministic single-photon sources remain difficult to manufacture at scale, and photon-photon interactions for two-qubit gates require probabilistic schemes or auxiliary systems. The path to fault-tolerant photonic quantum computing is longer than neutral-atom or superconducting approaches on current timelines — but the room-temperature and fiber-native properties make it uniquely suited to quantum networking applications.</p>
      <p>Japan has a 2030 national quantum roadmap. In its 2025 budget, the Japanese government allocated ¥1.05 trillion for next-generation chip and quantum computing research, encompassing computing, sensing, and communication programs across government, academic, and industry partners.</p>
    </div>
    <div>
      <div class="s9-specs">
        <div class="s9-spec"><span class="sp-label">Qubit type</span><span class="sp-val">Photonic</span></div>
        <div class="s9-spec"><span class="sp-label">Operating temp</span><span class="sp-val">~300K</span></div>
        <div class="s9-spec"><span class="sp-label">Key advantage</span><span class="sp-val">Fiber-native</span></div>
        <div class="s9-spec"><span class="sp-label">Lead orgs</span><span class="sp-val">NTT + NICT</span></div>
        <div class="s9-spec"><span class="sp-label">National allocation</span><span class="sp-val">¥1.05T</span></div>
        <div class="s9-spec"><span class="sp-label">Roadmap target</span><span class="sp-val">2030</span></div>
      </div>
    </div>
  </div>
</section>

<!-- ══════════════════════════════════════════════════════
     STORY 10 · FEATURE · Quantum Networking
═══════════════════════════════════════════════════════ -->
<section id="s10">
  <div class="s10-header">
    <span class="s10-eyebrow">Weird Science · Story 10 of 11</span>
    <h2 class="s10-hed">The Quantum<br><em>Internet</em> Is Closer<br>Than You Think</h2>
  </div>
  <div class="s10-body">
    <div>
      <div class="s10-text">
        <p>In Chicago, a 52-mile quantum network — the Chicago Quantum Exchange's testbed along an existing fiber-optic route — has demonstrated entanglement distribution between three nodes without classical memory as an intermediary. In Delft, researchers at TU Delft achieved memory-enhanced quantum communication over metropolitan distances, storing an entangled state in a nitrogen-vacancy center diamond memory for long enough to transmit the entanglement to a distant node and verify it. These are not demonstrations of a finished product. They are demonstrations that the pieces of a quantum internet are real.</p>
        <p>The quantum internet is often described as a future technology. It is more accurate to describe it as a present technology at laboratory scale, with well-understood engineering challenges between where we are and where we need to be. The core challenge is the quantum repeater: a device that can extend the range of entanglement distribution without amplifying the signal in the classical sense — because quantum states cannot be copied, only teleported.</p>
        <p>Several paths to quantum repeaters are now in active development. The most mature uses matter qubits — atoms or nitrogen-vacancy centers — as quantum memories. A photon arrives, its entanglement is stored in the memory, and another photon is generated to carry that entanglement further. The Delft group's results show that this basic architecture works. The remaining challenge is speed: current memories are too slow and too lossy to build a practical network at metropolitan, let alone intercontinental, scale.</p>
      </div>
      <p class="s10-pullquote">"We are not building a quantum internet. We are building the first fiber and the first switch. The network will take a generation."</p>
      <div class="s10-text">
        <p>The commercial case for a quantum internet is clearer than it might appear. Quantum key distribution — using entangled photons to distribute cryptographic keys that are physically impossible to intercept without detection — is already a commercial product sold by ID Quantique, Toshiba, and others. But QKD without a quantum repeater is limited to line-of-sight or short fiber distances. A quantum repeater network would enable QKD at continental scale: essentially unbreakable encryption for financial, government, and critical infrastructure communications.</p>
      </div>
    </div>
    <div>
      <!-- Network Graph SVG -->
      <div class="network-wrap">
        <svg viewBox="0 0 300 300" width="300" height="300" xmlns="http://www.w3.org/2000/svg">
          <defs>
            <filter id="net-glow"><feGaussianBlur stdDeviation="3" result="b"/><feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge></filter>
            <radialGradient id="node-grad"><stop offset="0%" stop-color="#2BAAFF"/><stop offset="100%" stop-color="#0055aa"/></radialGradient>
          </defs>
          <rect width="300" height="300" fill="#040c16"/>
          <!-- Network edges -->
          <g stroke="rgba(43,170,255,.2)" stroke-width="1.2">
            <line x1="150" y1="50" x2="50" y2="130"/>
            <line x1="150" y1="50" x2="250" y2="130"/>
            <line x1="150" y1="50" x2="150" y2="250"/>
            <line x1="50" y1="130" x2="250" y2="130"/>
            <line x1="50" y1="130" x2="150" y2="250"/>
            <line x1="250" y1="130" x2="150" y2="250"/>
            <line x1="50" y1="130" x2="30" y2="220"/>
            <line x1="250" y1="130" x2="270" y2="220"/>
            <line x1="150" y1="250" x2="30" y2="220"/>
            <line x1="150" y1="250" x2="270" y2="220"/>
          </g>
          <!-- Entanglement links (glowing) -->
          <g stroke="rgba(43,170,255,.6)" stroke-width="1.8" filter="url(#net-glow)" stroke-dasharray="4 3">
            <line x1="150" y1="50" x2="50" y2="130"/>
            <line x1="50" y1="130" x2="150" y2="250"/>
            <line x1="150" y1="250" x2="270" y2="220"/>
          </g>
          <!-- Nodes -->
          <g filter="url(#net-glow)">
            <circle cx="150" cy="50" r="12" fill="url(#node-grad)"/>
            <circle cx="50" cy="130" r="10" fill="#1a3a60"/>
            <circle cx="250" cy="130" r="10" fill="#1a3a60"/>
            <circle cx="150" cy="250" r="12" fill="url(#node-grad)"/>
            <circle cx="30" cy="220" r="8" fill="#0f2040"/>
            <circle cx="270" cy="220" r="8" fill="#0f2040"/>
          </g>
          <!-- Labels -->
          <text x="150" y="34" text-anchor="middle" font-family="JetBrains Mono,monospace" font-size="8.5" fill="rgba(43,170,255,.6)">Chicago</text>
          <text x="34" y="124" text-anchor="end" font-family="JetBrains Mono,monospace" font-size="8" fill="rgba(43,170,255,.4)">Argonne</text>
          <text x="266" y="124" text-anchor="start" font-family="JetBrains Mono,monospace" font-size="8" fill="rgba(43,170,255,.4)">Fermilab</text>
          <text x="150" y="272" text-anchor="middle" font-family="JetBrains Mono,monospace" font-size="8.5" fill="rgba(43,170,255,.6)">UChicago</text>
          <text x="150" y="296" text-anchor="middle" font-family="JetBrains Mono,monospace" font-size="8" fill="rgba(43,170,255,.25)" letter-spacing="2">CHICAGO QUANTUM EXCHANGE NETWORK</text>
        </svg>
      </div>
    </div>
  </div>
</section>

<!-- ══════════════════════════════════════════════════════
     STORY 11 · CLOSING HERO
═══════════════════════════════════════════════════════ -->
<section id="s11">
  <!-- Dawn horizon SVG (background) -->
  <svg style="position:absolute;bottom:0;left:0;width:100%;height:50%;opacity:.12" viewBox="0 0 1200 300" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg">
    <defs>
      <linearGradient id="dawn" x1="0" y1="0" x2="0" y2="1">
        <stop offset="0%" stop-color="#2BAAFF" stop-opacity="0"/>
        <stop offset="100%" stop-color="#2BAAFF" stop-opacity=".8"/>
      </linearGradient>
    </defs>
    <ellipse cx="600" cy="300" rx="500" ry="200" fill="url(#dawn)" class="dawn-line"/>
    <line x1="0" y1="300" x2="1200" y2="300" stroke="#2BAAFF" stroke-width="1" opacity=".4" class="dawn-line"/>
    <!-- Horizon rays -->
    <g stroke="rgba(43,170,255,.15)" stroke-width="1" class="dawn-line">
      <line x1="600" y1="300" x2="100" y2="0"/>
      <line x1="600" y1="300" x2="250" y2="0"/>
      <line x1="600" y1="300" x2="400" y2="0"/>
      <line x1="600" y1="300" x2="600" y2="0"/>
      <line x1="600" y1="300" x2="800" y2="0"/>
      <line x1="600" y1="300" x2="950" y2="0"/>
      <line x1="600" y1="300" x2="1100" y2="0"/>
    </g>
  </svg>
  <h2 class="s11-hed">
    The <span>Useful</span><br>Quantum<br><i style="font-style:italic;color:#888">Era.</i>
  </h2>
  <div class="s11-manifesto">
    <p class="manifesto-p"><strong>The question has changed.</strong> For thirty years, the dominant question in quantum computing was whether it would work at all — whether the physics was sound, whether the engineering was tractable, whether the error rates could be brought low enough for the machine to mean anything. That question has been answered. The answer is yes, under the right conditions, with the right hardware, in the right algorithmic domain. The question now is whether it will work for something real.</p>
    <p class="manifesto-p"><strong>The transition is already happening.</strong> Not in the dramatic, overnight way that technology transitions are described in retrospect, but in the slow, compounding way they actually occur: a pharmaceutical company runs a molecular simulation that its classical cluster cannot. A financial institution finds a portfolio optimization result that changes a hedging decision. A defense contractor gets a sensor reading that GPS could not have provided. Each of these is small. Their accumulation is not.</p>
    <p class="manifesto-p"><strong>World Quantum Day exists to mark the moment.</strong> April 14 — chosen because the fundamental quantum constant ℏ begins with the digits 4 and 14 — is a reminder that the field has a culture, a history, and a reason to celebrate its own progress. A year ago, this magazine would have been a collection of breakthroughs-in-waiting. Today it is something closer to a progress report. The useful quantum era has not fully arrived. But it is, unmistakably, arriving.</p>
  </div>
  <div class="s11-closer">
    <span class="s11-wordmark">The Quantum Record</span>
    <span style="color:#333;font-size:1rem">—</span>
    <span class="s11-date">Special Edition · April 14, 2026 · World Quantum Day</span>
  </div>
</section>

<!-- ══════════════════════════════════════════════════════
     FOOTER
═══════════════════════════════════════════════════════ -->
<footer>
  <div class="foot-col">
    <h4>About This Edition</h4>
    <p>The Quantum Record is a special-edition digital magazine produced for World Quantum Day 2026. All stories represent editorial synthesis of publicly available research, press releases, and industry reporting. The publication is independent and not affiliated with any of the organizations covered.</p>
  </div>
  <div class="foot-col">
    <h4>Stories in This Edition</h4>
    <ul>
      <li><span>01</span> The Logical Qubit Has Arrived</li>
      <li><span>02</span> Microsoft's Topological Gambit</li>
      <li><span>03</span> Willow's Warning Shot</li>
      <li><span>04</span> Britain Doubles Down</li>
      <li><span>05</span> The Mile-High Quantum Corridor</li>
      <li><span>06</span> Sensing the Unsensable</li>
      <li><span>07</span> Europe's Quantum Decade: Year Five</li>
      <li><span>08</span> Neutral-Atom Expansion</li>
      <li><span>09</span> Japan Goes Photonic</li>
      <li><span>10</span> The Quantum Internet</li>
      <li><span>11</span> The Useful Quantum Era</li>
    </ul>
  </div>
  <div class="foot-col">
    <h4>Themes Covered</h4>
    <ul>
      <li><span>·</span> Commercial Milestones</li>
      <li><span>·</span> Regional Ecosystems</li>
      <li><span>·</span> The Human Element</li>
      <li><span>·</span> Fault Tolerance &amp; Error Correction</li>
      <li><span>·</span> Quantum Sensing</li>
      <li><span>·</span> Quantum Networking</li>
      <li><span>·</span> National Quantum Programs</li>
    </ul>
    <p style="margin-top:24px;font-size:.78rem;color:#333">ℏ = 1.054571817 × 10⁻³⁴ J·s<br>April · 14 · 2026</p>
  </div>
</footer>

</body>
</html>
