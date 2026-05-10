<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Switch Direction — Business Coaching</title>
<style>
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:Arial,sans-serif;color:#1a1a2e;background:#fff}
:root{
  --purple:#4A2D7F;
  --purple-dark:#2e1a52;
  --gold:#B8982A;
  --gold-light:#E8D48A;
  --gold-pale:#F5EEC4;
  --gold-dark:#8A6E1A;
  --plat:#9BA8A0;
  --dark:#1A1A2E;
  --grey-bg:#f7f7f5;
  --border:#e0e0d8;
  --text-muted:#666;
}
.hero{background:var(--purple);color:#fff;padding:4rem 2rem;text-align:center}
.logo-mark{margin:0 auto 1rem;display:block}
.hero-logo-text{font-size:1.6rem;font-weight:700;color:#fff;margin-bottom:4px}
.hero-logo-sub{font-size:0.85rem;color:var(--gold-light);letter-spacing:1px;margin-bottom:1.5rem}
.divider{height:3px;background:linear-gradient(90deg,var(--purple),var(--gold),var(--plat));width:60px;margin:0 auto 1.5rem}
.hero-tag{font-size:11px;letter-spacing:3px;text-transform:uppercase;color:var(--gold-light);margin-bottom:1rem}
.hero h1{font-size:2.2rem;font-weight:700;line-height:1.25;color:#fff;margin-bottom:1rem;max-width:620px;margin-left:auto;margin-right:auto}
.hero p{font-size:1.05rem;color:rgba(255,255,255,0.78);max-width:500px;margin:0 auto 2rem}
.hero-btns{display:flex;gap:12px;justify-content:center;flex-wrap:wrap}
.btn-gold{background:var(--gold);color:#fff;border:none;padding:14px 32px;border-radius:8px;font-size:1rem;font-weight:600;cursor:pointer}
.btn-gold:hover{background:var(--gold-dark)}
.btn-outline{background:transparent;color:#fff;border:1.5px solid rgba(255,255,255,0.45);padding:13px 28px;border-radius:8px;font-size:1rem;cursor:pointer}
.btn-outline:hover{background:rgba(255,255,255,0.08)}
section{padding:3.5rem 2rem}
.container{max-width:740px;margin:0 auto}
.section-label{font-size:11px;letter-spacing:3px;text-transform:uppercase;color:var(--gold);font-weight:600;margin-bottom:0.75rem}
h2{font-size:1.75rem;font-weight:700;margin-bottom:1rem;color:#1a1a2e}
.pain{background:var(--grey-bg)}
.pain-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:16px;margin-top:2rem}
.pain-card{background:#fff;border:1px solid var(--border);border-top:3px solid var(--gold);border-radius:10px;padding:1.25rem}
.pain-card h3{font-size:1rem;font-weight:700;margin-bottom:0.4rem}
.pain-card p{font-size:0.875rem;color:var(--text-muted);line-height:1.6}
.programme{background:#fff}
.prog-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(160px,1fr));gap:12px;margin-top:2rem}
.prog-item{border:1px solid var(--border);border-radius:10px;padding:1.25rem;background:var(--purple);text-align:center}
.prog-num{font-size:2rem;font-weight:700;color:var(--gold-light)}
.prog-label{font-size:0.82rem;color:rgba(255,255,255,0.65);margin-top:4px}
.topics{margin-top:2rem}
.topic-row{display:flex;align-items:flex-start;gap:14px;padding:1rem 0;border-bottom:1px solid var(--border)}
.topic-row:last-child{border-bottom:none}
.topic-num{font-size:1rem;font-weight:700;color:var(--gold);min-width:24px;margin-top:2px}
.topic-row h4{font-size:0.95rem;font-weight:700;margin-bottom:0.2rem}
.topic-row p{font-size:0.875rem;color:var(--text-muted);line-height:1.6}
.pricing-section{background:var(--grey-bg)}
.pricing-grid{display:grid;grid-template-columns:1fr 1fr;gap:16px;margin-top:2rem}
.price-card{background:#fff;border:1px solid var(--border);border-radius:10px;padding:1.5rem}
.price-card.featured{background:var(--purple);border:2px solid var(--gold);position:relative}
.price-badge{position:absolute;top:-12px;left:50%;transform:translateX(-50%);background:var(--gold);color:#fff;font-size:11px;font-weight:600;padding:3px 14px;border-radius:20px;white-space:nowrap}
.price-label{font-size:11px;letter-spacing:2px;text-transform:uppercase;font-weight:600;margin-bottom:0.75rem;color:var(--gold)}
.price-card.featured .price-label{color:var(--gold-light)}
.price-amount{font-size:2rem;font-weight:700;color:#1a1a2e}
.price-card.featured .price-amount{color:#fff}
.price-sub{font-size:0.8rem;color:var(--text-muted);margin-top:4px}
.price-card.featured .price-sub{color:rgba(255,255,255,0.65)}
.price-saving{font-size:0.8rem;color:var(--gold);margin-top:4px;font-weight:600}
.price-card.featured .price-saving{color:var(--gold-light)}
.about{background:var(--purple);color:#fff;border-bottom:3px solid #B8982A}
.about .section-label{color:var(--gold-light)}
.about h2{color:#fff}
.about p{color:rgba(255,255,255,0.75);line-height:1.8;font-size:1rem;margin-bottom:1rem}
.about-box{border-left:3px solid var(--gold);padding:1rem 1.5rem;margin-top:1.5rem;background:rgba(255,255,255,0.06);border-radius:0 8px 8px 0}
.about-box p{color:rgba(255,255,255,0.75);margin:0;font-size:0.9rem}
.about-box strong{color:#fff}
.booking{background:var(--grey-bg);padding-top:2rem;border-top:3px solid #B8982A}
.booking-card{background:#fff;border:1px solid var(--border);border-radius:10px;padding:2rem;max-width:580px;margin:0 auto}
.form-row{margin-bottom:1.25rem}
.form-grid{display:grid;grid-template-columns:1fr 1fr;gap:16px}
label{display:block;font-size:0.85rem;color:var(--text-muted);margin-bottom:6px}
input,textarea,select{width:100%;padding:10px 14px;border:1px solid var(--border);border-radius:8px;font-size:0.95rem;background:#fafaf8;color:#1a1a2e;font-family:Arial,sans-serif}
textarea{height:100px;resize:vertical}
.submit-btn{width:100%;padding:14px;background:var(--purple);color:#fff;border:none;border-radius:8px;font-size:1rem;font-weight:600;cursor:pointer;margin-top:0.5rem}
.submit-btn:hover{background:var(--gold)}
.pricing-note{font-size:0.82rem;color:var(--text-muted);text-align:center;margin-top:1rem}
.success-msg{display:none;background:#eaf3de;border-radius:8px;padding:1rem;color:#3B6D11;font-size:0.9rem;text-align:center;margin-top:1rem;border:1px solid #c0dd97}
.footer{background:var(--purple);color:rgba(255,255,255,0.6);padding:2rem;text-align:center}
.footer-logo{font-size:1.1rem;font-weight:700;color:#fff;margin-bottom:4px}
.footer-sub{font-size:0.8rem;color:var(--gold-light);margin-bottom:1rem}
@media(max-width:520px){
  .hero h1{font-size:1.6rem}
  .pricing-grid,.form-grid{grid-template-columns:1fr}
  .price-badge{font-size:10px}
}
</style>
</head>
<body>

<div class="hero">
  <svg class="logo-mark" width="120" height="120" viewBox="0 0 80 80" fill="none" xmlns="http://www.w3.org/2000/svg">
    <path d="M40 12 C40 12 52 18 56 30 C60 42 52 50 52 50" stroke="#C9A84C" stroke-width="5" stroke-linecap="round" fill="none"/>
    <polygon points="54,46 58,56 48,54" fill="#C9A84C"/>
    <path d="M40 68 C40 68 28 62 24 50 C20 38 28 30 28 30" stroke="#9BA8A0" stroke-width="5" stroke-linecap="round" fill="none"/>
    <polygon points="26,34 22,24 32,26" fill="#9BA8A0"/>
    <path d="M12 40 C12 40 18 28 30 24 C42 20 50 28 50 28" stroke="#C9A84C" stroke-width="5" stroke-linecap="round" fill="none"/>
    <polygon points="46,26 56,22 54,32" fill="#C9A84C"/>
    <path d="M68 40 C68 40 62 52 50 56 C38 60 30 52 30 52" stroke="#9BA8A0" stroke-width="5" stroke-linecap="round" fill="none"/>
    <polygon points="34,54 24,58 26,48" fill="#9BA8A0"/>
  </svg>
  <div class="hero-logo-text">Switch Direction</div>
  <div class="hero-logo-sub">training centred on you</div>
  <div class="divider"></div>
  <p class="hero-tag" style="font-size:1.35rem;color:#C9A84C;letter-spacing:2px;font-weight:600">Business Coaching Accelerator</p>
  <h1>Start strong. Build smart. Find your direction.</h1>
  <p>Group coaching for founders navigating the real challenges of starting a business — finances, focus, and finding balance.</p>
  <div class="hero-btns">
    <button class="btn-gold" onclick="document.getElementById('pricing-section').scrollIntoView({behavior:'smooth'})">Reserve your place</button>
    <button class="btn-outline" onclick="document.getElementById('programme').scrollIntoView({behavior:'smooth'})">See how it works</button>
  </div>
</div>

<section class="pain">
  <div class="container">
    <p class="section-label">Who this is for</p>
    <h2>Starting a business is harder than anyone tells you</h2>
    <p style="color:var(--text-muted);line-height:1.8">You had the idea, the drive, the plan — but now you're in the thick of it. The money side is confusing, the hours are relentless, and it's hard to know if you're on the right track. You're not alone.</p>
    <div class="pain-grid">
      <div class="pain-card">
        <h3>Startup overwhelm</h3>
        <p>Too many decisions, not enough time. Learn how to focus on what actually moves the needle.</p>
      </div>
      <div class="pain-card">
        <h3>Grow and nurture</h3>
        <p>Building the right relationships, developing your team, and nurturing a business culture that helps you grow sustainably.</p>
      </div>
      <div class="pain-card">
        <h3>Understanding finances</h3>
        <p>Cash flow, pricing, margins — demystified. Get confident reading your numbers and making decisions from them.</p>
      </div>
      <div class="pain-card">
        <h3>Work-life balance</h3>
        <p>When work is everywhere, home suffers. Build boundaries that protect both your business and your wellbeing.</p>
      </div>
      <div style="grid-column:span 2;margin-top:4px;border-radius:10px;overflow:hidden;max-height:280px">
        <img src="https://images.pexels.com/photos/3153198/pexels-photo-3153198.jpeg?auto=compress&cs=tinysrgb&w=1200" alt="Two people having a business coaching conversation" style="width:100%;height:280px;object-fit:cover;object-position:center;display:block"/>
      </div>
    </div>
  </div>
</section>

<section class="programme" id="programme">
  <div class="container">
    <p class="section-label">The programme</p>
    <h2>12 months. Small group. Real results.</h2>
    <p style="color:var(--text-muted);line-height:1.8">This isn't a course — it's a coaching group built around honest conversation, shared experience, and practical progress. A small cohort means real connection and individual attention.</p>
    <div class="prog-grid">
      <div class="prog-item"><div class="prog-num">12</div><div class="prog-label">months of support</div></div>
      <div class="prog-item"><div class="prog-num">10</div><div class="prog-label">people max per group</div></div>
      <div class="prog-item"><div class="prog-num">£95</div><div class="prog-label">per person, per month</div></div>
    </div>
    <div class="topics">

      <div class="topic-row"><div class="topic-num">01</div><div>
        <h4>Getting through the early chaos</h4>
        <ul style="margin-top:0.5rem;padding-left:1rem;color:#666;font-size:0.875rem;line-height:2">
          <li>Define what "success" actually looks like for you — lifestyle, income needs, stress tolerance, exit goals</li>
          <li>Validate the problem, not just the idea — would someone pay to solve this now?</li>
          <li>Separate busy work from progress — sales conversations move the business forward, not logos and socials</li>
          <li>Document decisions from day one — assumptions, pricing logic, offers, brand choices</li>
        </ul>
      </div></div>

      <div class="topic-row"><div class="topic-num">02</div><div>
        <h4>Money made simple</h4>
        <ul style="margin-top:0.5rem;padding-left:1rem;color:#666;font-size:0.875rem;line-height:2">
          <li>Work out your personal financial runway — how long can you survive if income is irregular or zero?</li>
          <li>Set prices based on sustainability, not confidence — underpricing is driven by fear, not strategy</li>
          <li>Put basic legal and financial structure in place early — contracts, insurance, accounting setup</li>
        </ul>
      </div></div>

      <div class="topic-row"><div class="topic-num">03</div><div>
        <h4>Protecting your personal life</h4>
        <ul style="margin-top:0.5rem;padding-left:1rem;color:#666;font-size:0.875rem;line-height:2">
          <li>Decide what you will not do — clear boundaries on services, pricing floors, and client types prevent burnout</li>
          <li>Get honest about your weakest skill — ignoring it is more costly than outsourcing or learning it</li>
          <li>Create a simple operating rhythm — weekly review, monthly finances, quarterly goals</li>
        </ul>
      </div></div>

      <div class="topic-row"><div class="topic-num">04</div><div>
        <h4>Building for the long term</h4>
        <ul style="margin-top:0.5rem;padding-left:1rem;color:#666;font-size:0.875rem;line-height:2">
          <li>Plan how you'll generate leads before you need them — lead generation works best when you're not desperate</li>
          <li>Build a support system that isn't just cheerleaders — you need people who challenge your assumptions</li>
        </ul>
      </div></div>

    </div>
  </div>
</section>

<section class="pricing-section" id="pricing-section">
  <div class="container">
    <p class="section-label">Pricing</p>
    <h2>Flexible payment options</h2>
    <p style="color:var(--text-muted);line-height:1.8">Choose the option that works best for you. All prices are subject to VAT.</p>
    <div class="pricing-grid" id="pricing-grid">
      <div class="price-card" style="cursor:pointer" onclick="showPricingForm('monthly')">
        <div class="price-label">Monthly</div>
        <div class="price-amount">£95<span style="font-size:1rem;font-weight:400;color:var(--text-muted)">/mo</span></div>
        <div class="price-sub">+ VAT · £114 inc. VAT · 12 monthly payments</div>
        <div class="price-sub" style="margin-top:8px">£1,140 + VAT total · £1,368 inc. VAT</div>
        <div style="margin-top:1rem;font-size:0.85rem;color:var(--gold);font-weight:600">Select this option →</div>
      </div>
      <div class="price-card featured" style="cursor:pointer" onclick="showPricingForm('full')">
        <div class="price-badge">Save 10%</div>
        <div class="price-label">Pay in full</div>
        <div class="price-amount">£1,026</div>
        <div class="price-sub">+ VAT · £1,231.20 inc. VAT · one payment</div>
        <div class="price-saving">Save £114 + VAT vs monthly</div>
        <div style="margin-top:1rem;font-size:0.85rem;color:var(--gold-light);font-weight:600">Select this option →</div>
      </div>
    </div>

    <div id="pricing-form" style="display:none;margin-top:0">
      <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:1.25rem">
        <div>
          <div id="form-plan-label" style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--gold);font-weight:600;margin-bottom:4px"></div>
          <div id="form-plan-amount" style="font-size:1.5rem;font-weight:700;color:#1a1a2e"></div>
        </div>
        <button onclick="showPricingCards()" style="background:none;border:1px solid var(--border);border-radius:8px;padding:7px 14px;font-size:0.82rem;color:var(--text-muted);cursor:pointer">← Change option</button>
      </div>
      <div style="background:#fff;border:1px solid var(--border);border-radius:10px;padding:2rem">
        <div class="form-grid">
          <div class="form-row"><label>First name</label><input type="text" id="p-fname" placeholder="Jane"/></div>
          <div class="form-row"><label>Last name</label><input type="text" id="p-lname" placeholder="Smith"/></div>
        </div>
        <div class="form-row"><label>Email address</label><input type="email" id="p-email" placeholder="jane@yourbusiness.com"/></div>
        <div class="form-row"><label>Your business (or idea)</label><input type="text" id="p-biz" placeholder="e.g. freelance designer, new café owner..."/></div>
        <div class="form-row"><label>What's your biggest challenge right now?</label><textarea id="p-challenge" placeholder="Tell us a little about where you're at and what you're hoping to get from the programme..."></textarea></div>
        <button class="submit-btn" onclick="handlePricingSubmit()">Reserve my place</button>
        <div class="success-msg" id="p-success">Thank you! We'll be in touch within 2 working days to confirm your place.</div>
        <p class="pricing-note">All prices + VAT · Max 8 places per cohort</p>
      </div>
    </div>
    <div style="margin-top:2rem;padding:1.5rem;border:1px solid var(--border);border-left:3px solid var(--gold);border-radius:0 8px 8px 0;background:#fff">
      <p style="font-size:1rem;color:#1a1a2e;font-weight:600;margin-bottom:0.4rem">Not sure which option is right for you?</p>
      <p style="font-size:0.9rem;color:var(--text-muted);line-height:1.7;margin-bottom:1rem">We're happy to have a no-pressure conversation before you commit. Most people find it easier to decide once they've had a chance to ask a few questions.</p>
      <a href="mailto:enquiries@switchdirection.co.uk" style="padding:11px 28px;font-size:0.95rem;text-decoration:none;display:inline-block;background:var(--gold);color:#fff;border-radius:8px;font-weight:600">Get in touch</a>
    </div>
  </div>
</section>

<section class="about">
  <div class="container">
    <p class="section-label">About us</p>
    <h2>A catalyst for real change</h2>
    <p>Switch Direction isn't just a training company — it's a catalyst for transformation. Since 2017 we've helped individuals and organisations find their footing, build confidence, and grow in ways that actually last.</p>
    <p>Our business coaching programme brings that same ethos to founders and early-stage business owners. We believe coaching should be honest, practical, and built entirely around you — not a generic playbook.</p>

    <div style="display:grid;grid-template-columns:1fr;gap:16px;margin-top:2rem">
      <div style="border:1px solid rgba(255,255,255,0.15);border-top:3px solid var(--gold);border-radius:10px;padding:1.25rem">
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--gold-light);font-weight:600;margin-bottom:0.6rem">Our mission</div>
        <p style="color:rgba(255,255,255,0.78);font-size:0.9rem;line-height:1.7">To place the quality of your experience at the heart of everything we do — while helping you build a business that genuinely works for your life.</p>
      </div>
      <div style="border:1px solid rgba(255,255,255,0.15);border-top:3px solid var(--gold);border-radius:10px;padding:1.25rem">
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--gold-light);font-weight:600;margin-bottom:0.6rem">Our vision</div>
        <p style="color:rgba(255,255,255,0.78);font-size:0.9rem;line-height:1.7">To deliver high-quality coaching that adds tangible value — through strong relationships, practical delivery, and a genuine belief in the people we work with.</p>
      </div>
      <div style="border:1px solid rgba(255,255,255,0.15);border-top:3px solid var(--gold);border-radius:10px;padding:1.25rem">
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--gold-light);font-weight:600;margin-bottom:0.6rem">Our approach</div>
        <p style="color:rgba(255,255,255,0.78);font-size:0.9rem;line-height:1.7">We protect the individual, encourage participation at a pace you're comfortable with, and believe in building lasting relationships — not just delivering sessions.</p>
      </div>
      <div style="border:1px solid rgba(255,255,255,0.15);border-top:3px solid var(--gold);border-radius:10px;padding:1.25rem">
        <div style="font-size:11px;letter-spacing:2px;text-transform:uppercase;color:var(--gold-light);font-weight:600;margin-bottom:0.6rem">Your journey</div>
        <p style="color:rgba(255,255,255,0.78);font-size:0.9rem;line-height:1.7">No two founders are the same. We take the time to understand where you're starting from, what success looks like for you, and how to get there — at a pace that fits your life.</p>
      </div>
    </div>

    <div class="about-box" style="margin-top:2rem">
      <p><strong>Based in Ipswich, Suffolk</strong><br>Switch Direction Group Ltd has supported businesses and individuals across the UK since 2017 — helping people at every level find clarity, confidence, and a direction worth heading in.</p>
    </div>


  </div>
</section>



<div class="footer">
  <svg width="70" height="70" viewBox="0 0 80 80" fill="none" xmlns="http://www.w3.org/2000/svg" style="margin-bottom:0.75rem">
    <g opacity="0.95">
      <path d="M40 12 C40 12 52 18 56 30 C60 42 52 50 52 50" stroke="#C9A84C" stroke-width="5" stroke-linecap="round" fill="none"/>
      <polygon points="54,46 58,56 48,54" fill="#C9A84C"/>
      <path d="M40 68 C40 68 28 62 24 50 C20 38 28 30 28 30" stroke="#9BA8A0" stroke-width="5" stroke-linecap="round" fill="none"/>
      <polygon points="26,34 22,24 32,26" fill="#9BA8A0"/>
      <path d="M12 40 C12 40 18 28 30 24 C42 20 50 28 50 28" stroke="#C9A84C" stroke-width="5" stroke-linecap="round" fill="none"/>
      <polygon points="46,26 56,22 54,32" fill="#C9A84C"/>
      <path d="M68 40 C68 40 62 52 50 56 C38 60 30 52 30 52" stroke="#9BA8A0" stroke-width="5" stroke-linecap="round" fill="none"/>
      <polygon points="34,54 24,58 26,48" fill="#9BA8A0"/>
    </g>
  </svg>
  <div class="footer-logo">Switch Direction Group Ltd</div>
  <div class="footer-sub">training centred on you</div>
  <p>Business coaching for founders who mean business.</p>
  <p style="margin-top:1.25rem;font-size:0.9rem">
    <a href="mailto:enquiries@switchdirection.co.uk" style="color:var(--gold-light);text-decoration:none">enquiries@switchdirection.co.uk</a>
    &nbsp;&nbsp;|&nbsp;&nbsp;
    <a href="tel:01473924242" style="color:var(--gold-light);text-decoration:none">01473 924242</a>
  </p>
  <p style="margin-top:0.75rem;font-size:0.78rem;opacity:0.5">© 2026 Switch Direction Group Ltd · Company No. 16175629 · VAT No. 484 6279 47</p>
</div>

<script>
function showPricingForm(plan){
  var grid=document.getElementById('pricing-grid');
  var form=document.getElementById('pricing-form');
  grid.style.transition='opacity 0.35s ease';
  grid.style.opacity='0';
  setTimeout(function(){
    grid.style.display='none';
    form.style.opacity='0';
    form.style.display='block';
    setTimeout(function(){
      form.style.transition='opacity 0.35s ease';
      form.style.opacity='1';
    },20);
  },350);
  if(plan==='monthly'){
    document.getElementById('form-plan-label').textContent='Monthly payment';
    document.getElementById('form-plan-amount').textContent='£95 + VAT (£114 inc. VAT) per month';
  } else {
    document.getElementById('form-plan-label').textContent='Pay in full — save 10%';
    document.getElementById('form-plan-amount').textContent='£1,026 + VAT (£1,231.20 inc. VAT)';
  }
}
function showPricingCards(){
  var grid=document.getElementById('pricing-grid');
  var form=document.getElementById('pricing-form');
  form.style.transition='opacity 0.35s ease';
  form.style.opacity='0';
  setTimeout(function(){
    form.style.display='none';
    grid.style.opacity='0';
    grid.style.display='grid';
    setTimeout(function(){
      grid.style.transition='opacity 0.35s ease';
      grid.style.opacity='1';
    },20);
  },350);
}
async function handlePricingSubmit(){
  var f=document.getElementById('p-fname').value;
  var e=document.getElementById('p-email').value;
  var l=document.getElementById('p-lname').value;
  var biz=document.getElementById('p-biz').value;
  var challenge=document.getElementById('p-challenge').value;
  var plan=document.getElementById('form-plan-amount').textContent;
  if(!f||!e){alert('Please fill in your name and email to continue.');return;}
  var btn=document.querySelector('#pricing-form .submit-btn');
  btn.textContent='Sending...';
  btn.disabled=true;
  btn.style.opacity='0.7';
  try{
    var res=await fetch('https://formspree.io/f/xwvyblzn',{
      method:'POST',
      headers:{'Content-Type':'application/json','Accept':'application/json'},
      body:JSON.stringify({
        'First name':f,
        'Last name':l,
        'Email':e,
        'Business':biz,
        'Payment option':plan,
        'Biggest challenge':challenge
      })
    });
    if(res.ok){
      document.getElementById('p-success').style.display='block';
      btn.style.opacity='0.5';
      btn.textContent='Submitted';
    } else {
      alert('Something went wrong — please email us directly at enquiries@switchdirection.co.uk');
      btn.disabled=false;btn.style.opacity='1';btn.textContent='Reserve my place';
    }
  } catch(err){
    alert('Something went wrong — please email us directly at enquiries@switchdirection.co.uk');
    btn.disabled=false;btn.style.opacity='1';btn.textContent='Reserve my place';
  }
}
function handleSubmit(){
  var f=document.getElementById('fname').value;
  var e=document.getElementById('email').value;
  if(!f||!e){alert('Please fill in your name and email to continue.');return;}
  document.getElementById('success').style.display='block';
  document.querySelector('.submit-btn').disabled=true;
  document.querySelector('.submit-btn').style.opacity='0.5';
}
</script>
</body>
</html>
