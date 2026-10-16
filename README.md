# nxtlvll-site.index.html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>NXT LVLL Consultancy — People &amp; Business Operations</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,300;9..144,400;9..144,500;9..144,600;9..144,700&family=Inter:wght@300;400;500;600;700&family=IBM+Plex+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#0B0C09;
    --bg-elevated:#16170F;
    --bg-card:#1B1C13;
    --paper:#F5F2E8;
    --paper-soft:#A7A597;
    --gold:#F2C14E;
    --gold-deep:#C8952F;
    --emerald:#2F6D5C;
    --line:rgba(245,242,232,0.13);
    --line-strong:rgba(245,242,232,0.24);
  }

  *{margin:0;padding:0;box-sizing:border-box;}
  html{scroll-behavior:smooth;}

  body{
    background:var(--bg);
    color:var(--paper);
    font-family:'Inter',sans-serif;
    font-weight:400;
    line-height:1.6;
    overflow-x:hidden;
  }

  a{color:inherit;text-decoration:none;}

  .wrap{max-width:1200px;margin:0 auto;padding:0 32px;}

  h1,h2,h3{
    font-family:'Fraunces',serif;
    font-weight:600;
    letter-spacing:-0.015em;
    color:var(--paper);
  }

  .gold-text{
    background:linear-gradient(100deg,var(--gold) 0%,var(--gold-deep) 60%,var(--gold) 100%);
    -webkit-background-clip:text;
    background-clip:text;
    color:transparent;
  }

  .eyebrow{
    font-family:'IBM Plex Mono',monospace;
    font-size:12px;
    letter-spacing:0.16em;
    text-transform:uppercase;
    color:var(--paper-soft);
  }

  .logo-mark{display:flex;align-items:center;gap:10px;}
  .logo-icon{width:30px;height:30px;flex-shrink:0;}
  .logo-word{font-family:'Fraunces',serif;font-size:19px;font-weight:700;letter-spacing:0.01em;color:var(--paper);}
  .logo-word span{
    background:linear-gradient(100deg,var(--gold),var(--gold-deep));
    -webkit-background-clip:text;background-clip:text;color:transparent;
  }

  nav{
    position:fixed;top:0;left:0;right:0;z-index:100;
    background:rgba(11,12,9,0.82);
    backdrop-filter:blur(12px);
    border-bottom:1px solid var(--line);
  }
  .nav-inner{max-width:1200px;margin:0 auto;padding:18px 32px;display:flex;justify-content:space-between;align-items:center;}
  .nav-links{display:flex;gap:36px;font-size:14px;color:var(--paper-soft);}
  .nav-links a{transition:color .25s ease;}
  .nav-links a:hover{color:var(--paper);}
  .nav-cta{font-size:13.5px;padding:10px 22px;border:1px solid var(--gold-deep);color:var(--gold);border-radius:2px;transition:all .25s ease;}
  .nav-cta:hover{background:var(--gold);color:#0B0C09;box-shadow:0 0 24px rgba(242,193,78,0.35);}
  @media(max-width:780px){ .nav-links{display:none;} }

  header.hero{padding:200px 0 140px;position:relative;overflow:hidden;}
  .hero-glow{position:absolute;top:-200px;right:-160px;width:640px;height:640px;background:radial-gradient(circle,rgba(242,193,78,0.16) 0%,rgba(242,193,78,0) 70%);pointer-events:none;}
  .hero-glow-2{position:absolute;bottom:-260px;left:-200px;width:560px;height:560px;background:radial-gradient(circle,rgba(47,109,92,0.22) 0%,rgba(47,109,92,0) 70%);pointer-events:none;}
  .grid-lines{
    position:absolute;inset:0;
    background-image:linear-gradient(var(--line) 1px, transparent 1px);
    background-size:100% 96px;
    -webkit-mask-image:linear-gradient(to bottom, rgba(0,0,0,0.5), transparent 70%);
    mask-image:linear-gradient(to bottom, rgba(0,0,0,0.5), transparent 70%);
    pointer-events:none;
  }
  .hero-eyebrow{margin-bottom:24px;display:flex;align-items:center;gap:12px;position:relative;z-index:2;}
  .hero-eyebrow .dash{width:28px;height:1px;background:var(--line-strong);}
  h1.headline{font-size:clamp(42px,6.8vw,92px);line-height:0.96;max-width:960px;font-weight:600;position:relative;z-index:2;}
  .hero-sub{margin-top:30px;max-width:540px;font-size:17.5px;color:var(--paper-soft);position:relative;z-index:2;}
  .hero-actions{margin-top:46px;display:flex;gap:16px;flex-wrap:wrap;position:relative;z-index:2;}
  .btn-primary{
    background:linear-gradient(100deg,var(--gold),var(--gold-deep));
    color:#171106;font-weight:600;padding:16px 30px;font-size:14px;border-radius:2px;display:inline-block;
    transition:transform .25s ease, box-shadow .25s ease;
  }
  .btn-primary:hover{transform:translateY(-2px);box-shadow:0 8px 30px rgba(242,193,78,0.28);}
  .btn-ghost{padding:16px 30px;font-size:14px;border:1px solid var(--line-strong);color:var(--paper);border-radius:2px;display:inline-block;transition:border-color .25s ease, color .25s ease;}
  .btn-ghost:hover{border-color:var(--paper);color:var(--paper);}

  .strip{border-top:1px solid var(--line);border-bottom:1px solid var(--line);padding:20px 0;font-family:'IBM Plex Mono',monospace;font-size:12px;letter-spacing:0.08em;text-transform:uppercase;color:var(--paper-soft);}
  .strip-inner{display:flex;justify-content:space-between;width:100%;flex-wrap:wrap;gap:12px;}
  .strip-inner span::before{content:"—";color:var(--paper-soft);margin-right:8px;}

  section{padding:130px 0;}
  .section-head{max-width:680px;margin-bottom:64px;}
  .section-head h2{font-size:clamp(28px,3.6vw,46px);margin-top:16px;}

  .scrollytelling{
    display:grid;
    grid-template-columns:280px 1fr;
    gap:80px;
    border-top:1px solid var(--line);
    padding-top:8px;
  }
  .sticky-panel{
    position:sticky;
    top:140px;
    align-self:start;
    height:fit-content;
    padding-top:56px;
  }
  .sticky-num{
    font-family:'IBM Plex Mono',monospace;
    font-size:14px;
    color:var(--paper-soft);
    margin-bottom:10px;
    transition:opacity .3s ease;
  }
  .sticky-title{
    font-family:'Fraunces',serif;
    font-size:40px;
    font-weight:600;
    color:var(--paper);
    margin-bottom:10px;
    transition:opacity .3s ease;
  }
  .sticky-sub{
    font-size:14px;
    color:var(--paper-soft);
    margin-bottom:28px;
    transition:opacity .3s ease;
  }
  .sticky-track{width:56px;height:3px;background:var(--line);border-radius:2px;overflow:hidden;}
  .sticky-fill{
    height:100%;
    width:33%;
    background:linear-gradient(90deg,var(--emerald),var(--gold));
    box-shadow:0 0 12px rgba(242,193,78,0.3);
    transition:width .5s cubic-bezier(.16,1,.3,1);
  }

  .scroll-steps{display:flex;flex-direction:column;}
  .scroll-step{
    min-height:62vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    padding:40px 0;
    border-bottom:1px solid var(--line);
    opacity:0.32;
    transition:opacity .5s ease;
  }
  .scroll-step.active{opacity:1;}
  .scroll-step .step-label{
    font-family:'IBM Plex Mono',monospace;
    font-size:12px;
    letter-spacing:0.1em;
    text-transform:uppercase;
    color:var(--paper-soft);
    margin-bottom:14px;
  }
  .scroll-step p{
    font-family:'Fraunces',serif;
    font-size:26px;
    font-weight:500;
    line-height:1.4;
    color:var(--paper);
    max-width:520px;
  }

  @media(max-width:820px){
    .scrollytelling{grid-template-columns:1fr;gap:0;}
    .sticky-panel{position:relative;top:0;padding-top:32px;padding-bottom:16px;}
    .scroll-step{min-height:auto;opacity:1;padding:28px 0;}
    .scroll-step p{font-size:20px;}
  }


  .services-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:1px;background:var(--line);border:1px solid var(--line);}
  .service-card{background:var(--bg);padding:46px;transition:background .3s ease, box-shadow .3s ease;position:relative;}
  .service-card:hover{background:var(--bg-card);box-shadow:inset 0 1px 0 var(--line-strong);}
  .service-num{font-family:'IBM Plex Mono',monospace;font-size:12px;color:var(--paper-soft);margin-bottom:20px;display:block;}
  .service-card h3{font-size:22px;margin-bottom:12px;}
  .service-card p{font-size:14.5px;color:var(--paper-soft);max-width:380px;}
  .service-tag{margin-top:18px;display:inline-block;font-family:'IBM Plex Mono',monospace;font-size:11px;letter-spacing:0.06em;text-transform:uppercase;color:var(--emerald);background:rgba(47,109,92,0.16);padding:5px 10px;border-radius:2px;}
  @media(max-width:760px){ .services-grid{grid-template-columns:1fr;} .service-card{padding:34px;} }

  .addons{margin-top:56px;}
  .addons-head{display:flex;align-items:baseline;gap:18px;flex-wrap:wrap;margin-bottom:20px;}
  .addons-head p{font-size:14px;color:var(--paper-soft);}
  .addons-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:16px;}
  .addon-card{border:1px dashed var(--line-strong);padding:30px 34px;border-radius:2px;transition:border-color .3s ease, background .3s ease;}
  .addon-card:hover{border-color:var(--paper-soft);background:var(--bg-card);}
  .addon-card h3{font-size:19px;margin-bottom:8px;}
  .addon-card p{font-size:14px;color:var(--paper-soft);max-width:380px;}
  @media(max-width:760px){ .addons-grid{grid-template-columns:1fr;} }

  .expertise-row{display:grid;grid-template-columns:repeat(3,1fr);gap:1px;background:var(--line);border:1px solid var(--line);margin-top:1px;}
  .expertise-cell{background:var(--bg-elevated);padding:34px 30px;}
  .expertise-cell .eyebrow{display:block;margin-bottom:10px;}
  .expertise-cell p{font-size:14px;color:var(--paper-soft);}
  @media(max-width:760px){ .expertise-row{grid-template-columns:1fr;} }

  .about-split{display:grid;grid-template-columns:1fr 1fr;gap:80px;}
  .about-split p{font-size:16px;color:var(--paper-soft);margin-bottom:20px;}
  .about-split .big-quote{font-family:'Fraunces',serif;font-size:27px;font-weight:500;line-height:1.4;color:var(--paper);}
  @media(max-width:820px){ .about-split{grid-template-columns:1fr;gap:40px;} }

  .founder-block{display:grid;grid-template-columns:220px 1fr;gap:60px;align-items:start;border-top:1px solid var(--line);padding-top:64px;margin-top:64px;}
  .founder-avatar{width:180px;height:180px;border-radius:4px;background:linear-gradient(135deg,var(--emerald),var(--bg-card));border:1px solid var(--line-strong);display:flex;align-items:center;justify-content:center;position:relative;overflow:hidden;}
  .founder-avatar::after{content:"";position:absolute;inset:0;background:radial-gradient(circle at 30% 20%, rgba(47,109,92,0.22), transparent 60%);}
  .founder-initials{font-family:'Fraunces',serif;font-size:56px;font-weight:600;background:linear-gradient(100deg,var(--gold),var(--gold-deep));-webkit-background-clip:text;background-clip:text;color:transparent;position:relative;z-index:1;}
  .founder-name{font-size:26px;margin-bottom:4px;}
  .founder-title{font-family:'IBM Plex Mono',monospace;font-size:12px;letter-spacing:0.1em;text-transform:uppercase;color:var(--paper-soft);margin-bottom:22px;}
  .founder-bio{font-size:15.5px;color:var(--paper-soft);max-width:580px;margin-bottom:24px;}
  .founder-chips{display:flex;gap:10px;flex-wrap:wrap;}
  .founder-chip{font-family:'IBM Plex Mono',monospace;font-size:11px;letter-spacing:0.05em;text-transform:uppercase;color:var(--paper-soft);border:1px solid var(--line-strong);padding:7px 12px;border-radius:2px;}
  @media(max-width:700px){ .founder-block{grid-template-columns:1fr;} .founder-avatar{width:140px;height:140px;} .founder-initials{font-size:44px;} }

  /* ---------- TESTIMONIALS ---------- */
  .testimonial-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:1px;
    background:var(--line);
    border:1px solid var(--line);
  }
  .testimonial-card{
    background:var(--bg);
    padding:38px 34px;
    display:flex;
    flex-direction:column;
    justify-content:space-between;
    min-height:280px;
  }
  .testimonial-quote{
    font-family:'Fraunces',serif;
    font-style:italic;
    font-weight:400;
    font-size:17px;
    line-height:1.5;
    color:var(--paper);
  }
  .testimonial-meta{
    margin-top:28px;
    display:flex;
    align-items:center;
    gap:12px;
  }
  .testimonial-avatar{
    width:38px;
    height:38px;
    border-radius:50%;
    background:linear-gradient(135deg,var(--emerald),var(--bg-card));
    border:1px solid var(--line-strong);
    display:flex;
    align-items:center;
    justify-content:center;
    font-family:'IBM Plex Mono',monospace;
    font-size:12px;
    color:var(--gold);
    flex-shrink:0;
  }
  .testimonial-name{font-size:13.5px;color:var(--paper);font-weight:500;}
  .testimonial-role{font-size:12px;color:var(--paper-soft);}
  @media(max-width:820px){ .testimonial-grid{grid-template-columns:1fr;} }

  .cta-section{background:var(--bg-elevated);border:1px solid var(--line);border-radius:4px;padding:84px 60px;display:grid;grid-template-columns:1fr 1fr;gap:60px;position:relative;overflow:hidden;}
  .cta-glow{position:absolute;top:-140px;right:-140px;width:400px;height:400px;background:radial-gradient(circle,rgba(242,193,78,0.16),transparent 70%);pointer-events:none;}
  .cta-section h2{font-size:clamp(30px,4vw,48px);position:relative;z-index:1;}
  .cta-left p{margin-top:20px;color:var(--paper-soft);max-width:400px;font-size:15px;position:relative;z-index:1;}
  form{display:flex;flex-direction:column;gap:16px;position:relative;z-index:1;}
  .field label{display:block;font-family:'IBM Plex Mono',monospace;font-size:11px;text-transform:uppercase;letter-spacing:0.08em;color:var(--paper-soft);margin-bottom:8px;}
  .field input, .field textarea, .field select{width:100%;background:transparent;border:none;border-bottom:1px solid var(--line-strong);color:var(--paper);font-family:'Inter',sans-serif;font-size:15px;padding:10px 0;outline:none;transition:border-color .25s ease;}
  .field select option{color:#111;}
  .field input:focus, .field textarea:focus, .field select:focus{border-color:var(--paper);}
  .field textarea{resize:vertical;min-height:70px;}
  .submit-btn{margin-top:12px;background:linear-gradient(100deg,var(--gold),var(--gold-deep));color:#171106;border:none;padding:16px 26px;font-family:'Inter',sans-serif;font-size:14px;font-weight:600;border-radius:2px;cursor:pointer;transition:transform .25s ease, box-shadow .25s ease;align-self:flex-start;}
  .submit-btn:hover{transform:translateY(-1px);box-shadow:0 8px 26px rgba(242,193,78,0.28);}
  .form-note{font-size:12px;color:var(--paper-soft);margin-top:4px;}
  @media(max-width:820px){ .cta-section{grid-template-columns:1fr;padding:48px 28px;} }

  footer{padding:48px 0 60px;border-top:1px solid var(--line);display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:16px;font-size:13px;color:var(--paper-soft);}

  .fade-in{opacity:0;transform:translateY(18px);transition:opacity .8s ease, transform .8s ease;}
  .fade-in.visible{opacity:1;transform:translateY(0);}

  @media (prefers-reduced-motion: reduce){ *{transition:none !important;} }
</style>
</head>
<body>

<nav>
  <div class="nav-inner">
    <div class="logo-mark">
      <svg class="logo-icon" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
        <defs>
          <linearGradient id="lg1" x1="0" y1="32" x2="32" y2="0" gradientUnits="userSpaceOnUse">
            <stop offset="0" stop-color="#C8952F"/>
            <stop offset="1" stop-color="#F2C14E"/>
          </linearGradient>
        </defs>
        <rect x="3" y="20" width="5" height="9" rx="1" fill="url(#lg1)"/>
        <rect x="13.5" y="13" width="5" height="16" rx="1" fill="url(#lg1)"/>
        <rect x="24" y="4" width="5" height="25" rx="1" fill="url(#lg1)"/>
        <path d="M20.5 6L29 6L29 14.5" stroke="url(#lg1)" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/>
        <path d="M4 15L15 4L29 6" stroke="url(#lg1)" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
      </svg>
      <div class="logo-word">NXT <span>LVLL</span></div>
    </div>
    <div class="nav-links">
      <a href="#expertise">Expertise</a>
      <a href="#services">Services</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </div>
    <a href="#contact" class="nav-cta">Book a consult</a>
  </div>
</nav>

<header class="hero">
  <div class="grid-lines"></div>
  <div class="hero-glow"></div>
  <div class="hero-glow-2"></div>
  <div class="wrap">
    <div class="hero-eyebrow">
      <div class="dash"></div>
      <span class="eyebrow">HR &amp; Business Operations Consulting</span>
    </div>
    <h1 class="headline">Built to scale.<br>Run by <span class="gold-text">design.</span></h1>
    <p class="hero-sub">NXT LVLL Consultancy designs the HR systems, operating processes, and growth infrastructure that turn a fast-growing team into a well-run one — without slowing you down.</p>
    <div class="hero-actions">
      <a href="#contact" class="btn-primary">Book a consultation</a>
      <a href="#services" class="btn-ghost">See services</a>
    </div>
  </div>
</header>

<div class="strip">
  <div class="wrap">
    <div class="strip-inner">
      <span>People Operations</span>
      <span>Systems &amp; CRM</span>
      <span>Certification &amp; Compliance</span>
      <span>Business Launch Strategy</span>
      <span>Executive Training</span>
      <span>Keynote Speaking</span>
    </div>
  </div>
</div>

<section id="expertise">
  <div class="wrap">
    <div class="section-head fade-in">
      <span class="eyebrow">The Approach</span>
      <h2>Three levels, one solid foundation each.</h2>
    </div>

    <div class="scrollytelling">
      <div class="sticky-panel">
        <div class="sticky-num" id="stickyNum">01</div>
        <div class="sticky-title" id="stickyTitle">Foundation</div>
        <div class="sticky-sub" id="stickySub">Structure &amp; policy</div>
        <div class="sticky-track"><div class="sticky-fill" id="stickyFill"></div></div>
      </div>

      <div class="scroll-steps">
        <div class="scroll-step" data-num="01" data-title="Foundation" data-sub="Structure &amp; policy">
          <div class="step-label">LVL 01 — Foundation</div>
          <p>Role clarity, policy, and documentation — the groundwork that keeps a growing team accountable and compliant.</p>
        </div>
        <div class="scroll-step" data-num="02" data-title="Structure" data-sub="Systems &amp; process">
          <div class="step-label">LVL 02 — Structure</div>
          <p>Performance systems, org design, and the CRM or process backbone a team can run without you holding it together.</p>
        </div>
        <div class="scroll-step" data-num="03" data-title="Scale" data-sub="Growth &amp; readiness">
          <div class="step-label">LVL 03 — Scale</div>
          <p>Certification applications, launch strategy, and the operational readiness to take on bigger contracts and bigger teams.</p>
        </div>
      </div>
    </div>

    <div class="expertise-row fade-in">
      <div class="expertise-cell">
        <span class="eyebrow">Hands-on</span>
        <p>Performance review systems and org charts built and run for real teams, not just theory.</p>
      </div>
      <div class="expertise-cell">
        <span class="eyebrow">Technical</span>
        <p>CRM architecture, custom pipelines, and process documentation clients can operate on their own.</p>
      </div>
      <div class="expertise-cell">
        <span class="eyebrow">Detail-driven</span>
        <p>Certification and compliance applications prepared with the precision review boards expect.</p>
      </div>
    </div>
  </div>
</section>


<section id="services">
  <div class="wrap">
    <div class="section-head fade-in">
      <span class="eyebrow">Services</span>
      <h2>Where we plug in.</h2>
    </div>

    <div class="services-grid fade-in">
      <div class="service-card">
        <span class="service-num">01</span>
        <h3>People &amp; HR Operations</h3>
        <p>Performance management systems, peer review frameworks, and org design that keep a team aligned as it grows.</p>
        <span class="service-tag">Foundation → Structure</span>
      </div>
      <div class="service-card">
        <span class="service-num">02</span>
        <h3>Systems &amp; CRM Build</h3>
        <p>CRM architecture and pipeline design, set up once, documented clearly, handed off in a state your team can run.</p>
        <span class="service-tag">Structure</span>
      </div>
      <div class="service-card">
        <span class="service-num">03</span>
        <h3>Certification &amp; Compliance</h3>
        <p>Certification applications and compliance documentation prepared with the detail review boards look for.</p>
        <span class="service-tag">Scale</span>
      </div>
      <div class="service-card">
        <span class="service-num">04</span>
        <h3>Business Launch Strategy</h3>
        <p>Market research, service tier design, and registration guidance for founders building something new.</p>
        <span class="service-tag">Scale</span>
      </div>
      <div class="service-card">
        <span class="service-num">05</span>
        <h3>Executive Training</h3>
        <p>Practical leadership training for executives and managers, covering people management, accountability, and building a strong team culture.</p>
        <span class="service-tag">Structure → Scale</span>
      </div>
      <div class="service-card">
        <span class="service-num">06</span>
        <h3>Keynote Speaking</h3>
        <p>Talks for conferences, company events, and leadership retreats on HR, workplace culture, and building businesses that last.</p>
        <span class="service-tag">Scale</span>
      </div>
    </div>

    <div class="addons fade-in">
      <div class="addons-head">
        <span class="eyebrow">Add-ons</span>
        <p>Extras you can bolt onto any engagement.</p>
      </div>
      <div class="addons-grid">
        <div class="addon-card">
          <h3>Web Development</h3>
          <p>A clean, fast website for your business, built to match your brand and ready to take inquiries.</p>
        </div>
        <div class="addon-card">
          <h3>Social Media Management</h3>
          <p>Content planning, posting, and upkeep so your brand stays active without eating your week.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="about">
  <div class="wrap">
    <div class="about-split fade-in">
      <div>
        <span class="eyebrow">About</span>
        <p class="big-quote" style="margin-top:20px;">Growth doesn't stall from a lack of ambition. It stalls when nobody builds the systems to hold the weight of it.</p>
      </div>
      <div>
        <p>NXT LVLL Consultancy sits at the intersection of people and process — designing the HR systems, operating structure, and compliance groundwork that let founders and small teams scale without losing what made them work in the first place.</p>
        <p>Every engagement starts with an honest read of where things actually stand, then builds forward one level at a time: foundation, structure, scale.</p>
      </div>
    </div>

    <div class="founder-block fade-in">
      <div class="founder-avatar">
        <svg viewBox="0 0 32 32" width="72" height="72" fill="none" xmlns="http://www.w3.org/2000/svg" style="position:relative;z-index:1;" aria-hidden="true">
          <defs>
            <linearGradient id="lg2" x1="0" y1="32" x2="32" y2="0" gradientUnits="userSpaceOnUse">
              <stop offset="0" stop-color="#C8952F"/>
              <stop offset="1" stop-color="#F2C14E"/>
            </linearGradient>
          </defs>
          <rect x="3" y="20" width="5" height="9" rx="1" fill="url(#lg2)"/>
          <rect x="13.5" y="13" width="5" height="16" rx="1" fill="url(#lg2)"/>
          <rect x="24" y="4" width="5" height="25" rx="1" fill="url(#lg2)"/>
          <path d="M20.5 6L29 6L29 14.5" stroke="url(#lg2)" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"/>
          <path d="M4 15L15 4L29 6" stroke="url(#lg2)" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
        </svg>
      </div>
      <div>
        <h3 class="founder-name">Our team and company</h3>
        <div class="founder-title">NXT LVLL Consultancy</div>
        <p class="founder-bio">We bring over 10 years of HR and operations experience across small businesses and larger corporations. Our specialty is a 360° read on your business: what it needs on the people side and the operational side to run at its full potential.</p>
        <div class="founder-chips">
          <span class="founder-chip">10+ Years Experience</span>
          <span class="founder-chip">HR &amp; Operations</span>
          <span class="founder-chip">360° Business Analysis</span>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="testimonials">
  <div class="wrap">
    <div class="section-head fade-in">
      <span class="eyebrow">In Their Words</span>
      <h2>What it's like to work together.</h2>
    </div>

    <div class="testimonial-grid fade-in">
      <div class="testimonial-card">
        <div class="testimonial-quote">"I went in thinking I just needed a handbook. The review showed me the gaps in how we actually operate, then we fixed them."</div>
        <div class="testimonial-meta">
          <div>
            <div class="testimonial-name">Founder, boutique agency</div>
            <div class="testimonial-role">Toronto</div>
          </div>
        </div>
      </div>
      <div class="testimonial-card">
        <div class="testimonial-quote">"Our CRM finally makes sense. Everything's documented well enough that new hires figure it out on their own."</div>
        <div class="testimonial-meta">
          <div>
            <div class="testimonial-name">Operations lead, small business</div>
            <div class="testimonial-role">Brampton</div>
          </div>
        </div>
      </div>
      <div class="testimonial-card">
        <div class="testimonial-quote">"Detail-oriented without being slow. My certification application was ready weeks ahead of schedule."</div>
        <div class="testimonial-meta">
          <div>
            <div class="testimonial-name">Owner, consulting practice</div>
            <div class="testimonial-role">Mississauga</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="contact">
  <div class="wrap">
    <div class="cta-section fade-in">
      <div class="cta-glow"></div>
      <div class="cta-left">
        <span class="eyebrow">Get Started</span>
        <h2>Ready for the<br>next level?</h2>
        <p>Tell me a bit about where your business stands right now — I'll follow up to schedule a consultation.</p>
      </div>
      <form id="consult-form">
        <div class="field">
          <label for="name">Name</label>
          <input type="text" id="name" required>
        </div>
        <div class="field">
          <label for="email">Email</label>
          <input type="email" id="email" required>
        </div>
        <div class="field">
          <label for="service">What do you need help with?</label>
          <select id="service">
            <option>People &amp; HR Operations</option>
            <option>Systems &amp; CRM Build</option>
            <option>Certification &amp; Compliance</option>
            <option>Business Launch Strategy</option>
            <option>Executive Training</option>
            <option>Keynote Speaking</option>
            <option>Add-on: Web Development</option>
            <option>Add-on: Social Media Management</option>
            <option>Not sure yet</option>
          </select>
        </div>
        <div class="field">
          <label for="message">A bit about your business</label>
          <textarea id="message" rows="3"></textarea>
        </div>
        <button type="submit" class="submit-btn">Request a consultation</button>
        <div class="form-note" id="form-note">Opens a pre-filled email in Gmail — nothing sends automatically.</div>
      </form>
    </div>
  </div>
</section>

<footer>
  <div class="wrap" style="display:flex;justify-content:space-between;width:100%;flex-wrap:wrap;gap:16px;">
    <div>NXT LVLL Consultancy © 2026</div>
    <div>hello@nxtlvllconsultancy.com</div>
  </div>
</footer>

<script>
  const faders = document.querySelectorAll('.fade-in');
  const io = new IntersectionObserver((entries)=>{
    entries.forEach(e=>{
      if(e.isIntersecting){
        e.target.classList.add('visible');
        io.unobserve(e.target);
      }
    });
  },{threshold:0.15});
  faders.forEach(f=>io.observe(f));

  // scrollytelling: sticky panel updates as each step scrolls through view
  const scrollSteps = document.querySelectorAll('.scroll-step');
  const stickyNum = document.getElementById('stickyNum');
  const stickyTitle = document.getElementById('stickyTitle');
  const stickySub = document.getElementById('stickySub');
  const stickyFill = document.getElementById('stickyFill');
  const totalSteps = scrollSteps.length;

  const stepObserver = new IntersectionObserver((entries)=>{
    entries.forEach(entry=>{
      if(entry.isIntersecting){
        scrollSteps.forEach(s=>s.classList.remove('active'));
        entry.target.classList.add('active');

        const num = entry.target.getAttribute('data-num');
        const title = entry.target.getAttribute('data-title');
        const sub = entry.target.getAttribute('data-sub');
        const index = Array.from(scrollSteps).indexOf(entry.target);

        [stickyNum, stickyTitle, stickySub].forEach(el=>el.style.opacity='0');
        setTimeout(()=>{
          stickyNum.textContent = num;
          stickyTitle.textContent = title;
          stickySub.textContent = sub;
          [stickyNum, stickyTitle, stickySub].forEach(el=>el.style.opacity='1');
        }, 150);

        stickyFill.style.width = (((index+1)/totalSteps)*100) + '%';
      }
    });
  },{threshold:0.5, rootMargin:'-20% 0px -20% 0px'});

  scrollSteps.forEach(s=>stepObserver.observe(s));

  const DESTINATION_EMAIL = "hello@nxtlvllconsultancy.com";
  const form = document.getElementById('consult-form');
  const note = document.getElementById('form-note');

  form.addEventListener('submit', function(ev){
    ev.preventDefault();
    const name = document.getElementById('name').value.trim();
    const email = document.getElementById('email').value.trim();
    const service = document.getElementById('service').value;
    const message = document.getElementById('message').value.trim();

    const subject = `Consultation request — ${name}`;
    const body =
`Name: ${name}
Email: ${email}
Area of interest: ${service}

${message}`;

    const gmailUrl =
      "https://mail.google.com/mail/?view=cm&fs=1" +
      "&to=" + encodeURIComponent(DESTINATION_EMAIL) +
      "&su=" + encodeURIComponent(subject) +
      "&body=" + encodeURIComponent(body);

    window.open(gmailUrl, "_blank");
    note.textContent = "Opening Gmail in a new tab with your details filled in — just hit send.";
    note.style.color = "var(--gold)";
  });
</script>

</body>
</html>
