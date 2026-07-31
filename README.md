# adam-moummou
Emplacement magnifique
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ADAM MOUMMOU | شحن جواهر Free Fire</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Cinzel:wght@500;700;900&family=Tajawal:wght@400;500;700;900&display=swap');

  * { margin:0; padding:0; box-sizing:border-box; }

  html { scroll-behavior:smooth; }

  body {
    background:#0a0806;
    color:#f2ead9;
    font-family:'Tajawal', sans-serif;
    overflow-x:hidden;
    position:relative;
  }

  .bg-glow {
    position:fixed;
    inset:0;
    z-index:0;
    background:
      radial-gradient(ellipse 600px 400px at 20% 10%, rgba(212,175,90,0.10), transparent 60%),
      radial-gradient(ellipse 700px 500px at 85% 25%, rgba(196,30,30,0.14), transparent 60%),
      radial-gradient(ellipse 800px 600px at 50% 90%, rgba(212,175,90,0.08), transparent 60%);
    pointer-events:none;
  }

  .particle {
    position:fixed;
    z-index:0;
    border-radius:2px;
    background: linear-gradient(135deg, #f4e2a1, #d4af5a);
    opacity:0.55;
    animation: floatUp linear infinite;
    pointer-events:none;
  }
  @keyframes floatUp {
    0%   { transform: translateY(110vh) rotate(0deg); opacity:0; }
    10%  { opacity:0.6; }
    90%  { opacity:0.4; }
    100% { transform: translateY(-10vh) rotate(360deg); opacity:0; }
  }

  section, header, footer { position:relative; z-index:1; }

  nav {
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:18px 6vw;
    position:sticky;
    top:0;
    z-index:50;
    backdrop-filter: blur(10px);
    background: rgba(10,8,6,0.65);
    border-bottom:1px solid rgba(212,175,90,0.15);
  }
  .brand {
    display:flex;
    align-items:center;
    gap:10px;
    font-family:'Cinzel', serif;
    font-weight:700;
    letter-spacing:0.06em;
    font-size:1.1rem;
    background: linear-gradient(100deg,#8a6c2f,#f4e2a1,#d4af5a,#fff6d6,#d4af5a,#8a6c2f);
    background-size:250% 100%;
    -webkit-background-clip:text;
    background-clip:text;
    color:transparent;
    animation: shine 5s linear infinite;
  }
  @keyframes shine {
    0% { background-position:200% 0%; }
    100% { background-position:-200% 0%; }
  }
  .brand svg { width:26px; height:auto; filter:drop-shadow(0 0 6px rgba(212,175,90,0.5)); }

  .nav-links { display:flex; gap:26px; }
  .nav-links a {
    color:#e8dcc0;
    text-decoration:none;
    font-size:0.92rem;
    font-weight:500;
    opacity:0.85;
    transition:.25s;
  }
  .nav-links a:hover { opacity:1; color:#f4e2a1; }

  .nav-cta {
    background: linear-gradient(135deg,#c41e1e,#8f1414);
    color:#fff;
    padding:9px 20px;
    border-radius:30px;
    font-size:0.88rem;
    font-weight:700;
    text-decoration:none;
    box-shadow:0 4px 18px rgba(196,30,30,0.35);
    transition:.25s;
  }
  .nav-cta:hover { transform:translateY(-2px); box-shadow:0 6px 22px rgba(196,30,30,0.5); }

  @media (max-width:720px){ .nav-links{ display:none; } }

  .hero {
    min-height:88vh;
    display:flex;
    flex-direction:column;
    align-items:center;
    justify-content:center;
    text-align:center;
    padding:80px 6vw 60px;
  }

  .crown {
    width:70px;
    margin-bottom:14px;
    filter: drop-shadow(0 0 12px rgba(212,175,90,0.55));
    animation: crownFloat 3.5s ease-in-out infinite;
  }
  @keyframes crownFloat {
    0%,100% { transform: translateY(0) rotate(0deg); }
    50%     { transform: translateY(-6px) rotate(1.5deg); }
  }

  .hero h1 {
    font-family:'Cinzel', serif;
    font-weight:900;
    font-size: clamp(2.2rem, 7vw, 4rem);
    letter-spacing:0.05em;
    background: linear-gradient(100deg,#8a6c2f,#f4e2a1,#d4af5a,#fff6d6,#d4af5a,#8a6c2f);
    background-size:250% 100%;
    -webkit-background-clip:text;
    background-clip:text;
    color:transparent;
    animation: shine 5s linear infinite;
    margin-bottom:6px;
  }

  .hero .tagline {
    font-size:clamp(1rem,2.6vw,1.35rem);
    color:#e8dcc0;
    opacity:0.9;
    margin-bottom:28px;
  }
  .hero .tagline b { color:#ff4d4d; }

  .badges {
    display:flex;
    gap:14px;
    flex-wrap:wrap;
    justify-content:center;
    margin-bottom:36px;
  }
  .badge {
    display:flex;
    align-items:center;
    gap:8px;
    background: rgba(212,175,90,0.08);
    border:1px solid rgba(212,175,90,0.3);
    padding:8px 16px;
    border-radius:30px;
    font-size:0.85rem;
    color:#f4e2a1;
  }

  .hero-cta {
    display:inline-flex;
    align-items:center;
    gap:10px;
    background: linear-gradient(135deg,#c41e1e,#8f1414);
    color:#fff;
    padding:15px 34px;
    border-radius:40px;
    font-weight:700;
    font-size:1.05rem;
    text-decoration:none;
    box-shadow:0 8px 28px rgba(196,30,30,0.4);
    transition:.25s;
    animation: pulseCta 2.4s ease-in-out infinite;
  }
  .hero-cta:hover { transform:translateY(-3px) scale(1.03); }
  @keyframes pulseCta {
    0%,100% { box-shadow:0 8px 28px rgba(196,30,30,0.4); }
    50%     { box-shadow:0 8px 38px rgba(196,30,30,0.65); }
  }

  .section-title {
    text-align:center;
    font-family:'Cinzel', serif;
    font-weight:700;
    font-size:clamp(1.5rem,4vw,2.2rem);
    color:#f4e2a1;
    margin-bottom:8px;
  }
  .section-sub {
    text-align:center;
    color:#b3a68a;
    font-size:0.95rem;
    margin-bottom:44px;
  }

  .packages {
    padding:70px 6vw;
  }

  .pkg-grid {
    display:grid;
    grid-template-columns:repeat(auto-fit, minmax(210px,1fr));
    gap:22px;
    max-width:1100px;
    margin:0 auto;
  }

  .pkg-card {
    position:relative;
    background: linear-gradient(160deg, rgba(255,255,255,0.04), rgba(255,255,255,0.01));
    border:1px solid rgba(212,175,90,0.25);
    border-radius:18px;
    padding:30px 20px;
    text-align:center;
    transition:.3s;
    overflow:hidden;
  }
  .pkg-card::before {
    content:"";
    position:absolute;
    inset:0;
    background: radial-gradient(circle at 50% 0%, rgba(212,175,90,0.12), transparent 70%);
    opacity:0;
    transition:.3s;
  }
  .pkg-card:hover {
    transform:translateY(-8px);
    border-color:rgba(212,175,90,0.6);
    box-shadow:0 14px 34px rgba(0,0,0,0.4);
  }
  .pkg-card:hover::before { opacity:1; }

  .pkg-card.popular {
    border-color:rgba(196,30,30,0.6);
    box-shadow:0 0 0 1px rgba(196,30,30,0.3), 0 14px 34px rgba(0,0,0,0.4);
  }
  .popular-tag {
    position:absolute;
    top:12px;
    left:50%;
    transform:translateX(-50%);
    background: linear-gradient(135deg,#c41e1e,#8f1414);
    color:#fff;
    font-size:0.7rem;
    font-weight:700;
    padding:4px 14px;
    border-radius:20px;
    letter-spacing:0.05em;
  }

  .pkg-amount {
    font-family:'Cinzel', serif;
    font-weight:700;
    font-size:1.5rem;
    color:#fdf6e3;
    margin:16px 0 4px;
  }
  .pkg-amount span { color:#d4af5a; font-size:1rem; }

  .pkg-price {
    font-size:1.6rem;
    font-weight:900;
    color:#f4e2a1;
    margin:14px 0 18px;
  }
  .pkg-price small { font-size:0.9rem; color:#b3a68a; font-weight:500; }

  .pkg-order {
    display:inline-block;
    width:100%;
    background: rgba(212,175,90,0.12);
    color:#f4e2a1;
    border:1px solid rgba(212,175,90,0.4);
    padding:10px 0;
    border-radius:12px;
    text-decoration:none;
    font-weight:700;
    font-size:0.9rem;
    transition:.25s;
  }
  .pkg-order:hover {
    background: linear-gradient(135deg,#c41e1e,#8f1414);
    border-color:transparent;
    color:#fff;
  }

  .steps {
    padding:70px 6vw;
    background: linear-gradient(180deg, transparent, rgba(212,175,90,0.04), transparent);
  }
  .steps-grid {
    display:grid;
    grid-template-columns:repeat(auto-fit, minmax(220px,1fr));
    gap:26px;
    max-width:1000px;
    margin:0 auto;
  }
  .step {
    text-align:center;
    padding:20px;
  }
  .step-num {
    width:50px;
    height:50px;
    margin:0 auto 16px;
    border-radius:50%;
    display:flex;
    align-items:center;
    justify-content:center;
    font-family:'Cinzel', serif;
    font-weight:700;
    font-size:1.2rem;
    color:#0a0806;
    background: linear-gradient(135deg,#f4e2a1,#d4af5a);
    box-shadow:0 0 20px rgba(212,175,90,0.4);
  }
  .step h3 { font-size:1.05rem; color:#f4e2a1; margin-bottom:8px; }
  .step p { font-size:0.88rem; color:#b3a68a; line-height:1.6; }

  .trust {
    padding:60px 6vw;
    text-align:center;
  }
  .trust-grid {
    display:flex;
    flex-wrap:wrap;
    justify-content:center;
    gap:40px;
    max-width:900px;
    margin:36px auto 0;
  }
  .trust-item h4 {
    font-family:'Cinzel', serif;
    font-size:1.8rem;
    color:#f4e2a1;
  }
  .trust-item p { font-size:0.85rem; color:#b3a68a; margin-top:4px; }

  .footer-cta {
    padding:90px 6vw;
    text-align:center;
    background: radial-gradient(ellipse at center, rgba(196,30,30,0.08), transparent 70%);
  }
  .footer-cta h2 {
    font-family:'Cinzel', serif;
    font-size:clamp(1.6rem,4vw,2.4rem);
    color:#f4e2a1;
    margin-bottom:14px;
  }
  .footer-cta p { color:#b3a68a; margin-bottom:30px; }

  footer {
    padding:30px 6vw;
    text-align:center;
    border-top:1px solid rgba(212,175,90,0.15);
    color:#8a7d5f;
    font-size:0.82rem;
  }
  footer a { color:#d4af5a; text-decoration:none; }

  .ig-icon { width:1em; height:1em; vertical-align:-2px; margin-left:4px; }
</style>
</head>
<body>

<div class="bg-glow"></div>
<div id="particles"></div>

<nav>
  <div class="brand">
    <svg viewBox="0 0 100 70" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <linearGradient id="navGrad" x1="0%" y1="0%" x2="100%" y2="100%">
          <stop offset="0%" stop-color="#f4e2a1"/>
          <stop offset="100%" stop-color="#8a6c2f"/>
        </linearGradient>
      </defs>
      <path d="M5 60 L5 30 L25 45 L50 12 L75 45 L95 30 L95 60 Z" fill="url(#navGrad)" stroke="#7a5f28" stroke-width="2"/>
      <rect x="5" y="58" width="90" height="8" rx="2" fill="url(#navGrad)" stroke="#7a5f28" stroke-width="1.5"/>
    </svg>
    ADAM MOUMMOU
  </div>
  <div class="nav-links">
    <a href="#packages">الباقات</a>
    <a href="#steps">كيفاش تطلب</a>
    <a href="#trust">الثقة</a>
  </div>
  <a class="nav-cta" href="https://instagram.com/_.ada_q" target="_blank" rel="noopener">شحن</a>
</nav>

<header class="hero">
  <svg class="crown" viewBox="0 0 100 70" xmlns="http://www.w3.org/2000/svg">
    <defs>
      <linearGradient id="heroGrad" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" stop-color="#f4e2a1"/>
        <stop offset="45%" stop-color="#d4af5a"/>
        <stop offset="100%" stop-color="#8a6c2f"/>
      </linearGradient>
    </defs>
    <path d="M5 60 L5 30 L25 45 L50 12 L75 45 L95 30 L95 60 Z" fill="url(#heroGrad)" stroke="#7a5f28" stroke-width="1.5" stroke-linejoin="round"/>
    <rect x="5" y="58" width="90" height="8" rx="2" fill="url(#heroGrad)" stroke="#7a5f28" stroke-width="1.2"/>
    <circle cx="50" cy="10" r="5" fill="#f4e2a1" stroke="#8a6c2f" stroke-width="1"/>
    <circle cx="25" cy="43" r="4" fill="#f4e2a1" stroke="#8a6c2f" stroke-width="1"/>
    <circle cx="75" cy="43" r="4" fill="#f4e2a1" stroke="#8a6c2f" stroke-width="1"/>
  </svg>

  <h1>ADAM MOUMMOU</h1>
  <p class="tagline">شحن جواهر <b>Free Fire</b> بأرخص الأسعار وأسرع وقت 💎</p>

  <div class="badges">
    <span class="badge">⚡ توصيل فوري</span>
    <span class="badge">🔒 معاملة آمنة</span>
    <span class="badge">💯 أسعار تنافسية</span>
  </div>

  <a class="hero-cta" href="https://instagram.com/_.ada_q" target="_blank" rel="noopener">
    اطلب الشحن على انستغرام
    <svg class="ig-icon" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" width="20" height="20">
      <rect x="2" y="2" width="20" height="20" rx="6" stroke="white" stroke-width="2"/>
      <circle cx="12" cy="12" r="5" stroke="white" stroke-width="2"/>
      <circle cx="17.5" cy="6.5" r="1.2" fill="white"/>
    </svg>
  </a>
</header>

<section class="packages" id="packages">
  <div class="section-title">الباقات ديال الجواهر</div>
  <div class="section-sub">1$ = 100 جوهرة — اختار الباقة اللي تناسبك</div>

  <div class="pkg-grid">

    <div class="pkg-card">
      <div class="pkg-amount">100 <span>💎</span></div>
      <div class="pkg-price">1$ <small>USD</small></div>
      <a class="pkg-order" href="https://instagram.com/_.ada_q" target="_blank" rel="noopener">شحن</a>
    </div>

    <div class="pkg-card">
      <div class="pkg-amount">310 <span>💎</span></div>
      <div class="pkg-price">3.1$ <small>USD</small></div>
      <a class="pkg-order" href="https://instagram.com/_.ada_q" target="_blank" rel="noopener">شحن</a>
    </div>

    <div class="pkg-card popular">
      <span class="popular-tag">الأكثر طلباً</span>
      <div class="pkg-amount">520 <span>💎</span></div>
      <div class="pkg-price">5.2$ <small>USD</small></div>
      <a class="pkg-order" href="https://instagram.com/_.ada_q" target="_blank" rel="noopener">شحن</a>
    </div>

    <div class="pkg-card">
      <div class="pkg-amount">1000 <span>💎</span></div>
      <div class="pkg-price">10$ <small>USD</small></div>
      <a class="pkg-order" href="https://instagram.com/_.ada_q" target="_blank" rel="noopener">شحن</a>
    </div>

    <div class="pkg-card">
      <div class="pkg-amount">2200 <span>💎</span></div>
      <div class="pkg-price">22$ <small>USD</small></div>
      <a class="pkg-order" href="https://instagram.com/_.ada_q" target="_blank" rel="noopener">شحن</a>
    </div>

    <div class="pkg-card">
      <div class="pkg-amount">5000 <span>💎</span></div>
      <div class="pkg-price">50$ <small>USD</small></div>
      <a class="pkg-order" href="https://instagram.com/_.ada_q" target="_blank" rel="noopener">شحن</a>
    </div>

  </div>
</section>

<section class="steps" id="steps">
  <div class="section-title">كيفاش تطلب؟</div>
  <div class="section-sub">3 خطوات بسيطة وغادي توصلك الجواهر</div>

  <div class="steps-grid">
    <div class="step">
      <div class="step-num">1</div>
      <h3>اختار الباقة</h3>
      <p>شوف الباقات فوق وحدد شحال بغيتي من الجواهر</p>
    </div>
    <div class="step">
      <div class="step-num">2</div>
      <h3>تواصل معايا</h3>
      <p>راسلني على إنستغرام وعطيني ID ديال اللعبة ديالك</p>
    </div>
    <div class="step">
      <div class="step-num">3</div>
      <h3>خلص واستافد</h3>
      <p>بعد التأكيد ديال الدفع، الجواهر كتوصل ليك فأسرع وقت</p>
    </div>
  </div>
</section>

<section class="trust" id="trust">
  <div class="section-title">علاش تختارني؟</div>
  <div class="trust-grid">
    <div class="trust-item">
      <h4>⚡ سريع</h4>
      <p>توصيل ديال الجواهر فدقائق</p>
    </div>
    <div class="trust-item">
      <h4>🔒 آمن</h4>
      <p>ماكاينش أي خطر على الحساب ديالك</p>
    </div>
    <div class="trust-item">
      <h4>💬 دعم مباشر</h4>
      <p>غادي نكون معاك على طول من البداية للنهاية</p>
    </div>
  </div>
</section>

<section class="footer-cta">
  <h2>واجد تشحن الجواهر ديالك؟</h2>
  <p>راسلني دابا على إنستغرام وغادي نعاونك فالحين</p>
  <a class="hero-cta" href="https://instagram.com/_.ada_q" target="_blank" rel="noopener">
    راسلني على @_.ada_q
    <svg class="ig-icon" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" width="20" height="20">
      <rect x="2" y="2" width="20" height="20" rx="6" stroke="white" stroke-width="2"/>
      <circle cx="12" cy="12" r="5" stroke="white" stroke-width="2"/>
      <circle cx="17.5" cy="6.5" r="1.2" fill="white"/>
    </svg>
  </a>
</section>

<footer>
  © 2026 ADAM MOUMMOU — جميع الحقوق محفوظة | تواصل: <a href="https://instagram.com/_.ada_q" target="_blank" rel="noopener">@_.ada_q</a>
</footer>

<script>
  const container = document.getElementById('particles');
  const count = 26;
  for (let i = 0; i < count; i++) {
    const p = document.createElement('div');
    p.className = 'particle';
    const size = 3 + Math.random() * 4;
    p.style.width = size + 'px';
    p.style.height = size + 'px';
    p.style.left = Math.random() * 100 + 'vw';
    p.style.animationDuration = (8 + Math.random() * 10) + 's';
    p.style.animationDelay = (Math.random() * 10) + 's';
    container.appendChild(p);
  }
</script>

</body>
</html>
