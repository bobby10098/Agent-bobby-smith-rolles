<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>National Grant Support Initiative — Demo</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;900&display=swap" rel="stylesheet">

<style>
:root{
  --bg:#0a0f1f;
  --glass:rgba(255,255,255,.08);
  --accent:#4da3ff;
  --accent2:#7cffc4;
  --text:#eef2ff;
  --muted:#a7b1d6;
}
*{box-sizing:border-box}
body{
  margin:0;
  font-family:Inter,system-ui;
  background:
    radial-gradient(1200px 600px at 15% -10%,#1b2b6f,transparent),
    radial-gradient(900px 500px at 90% 10%,#103b7a,transparent),
    var(--bg);
  color:var(--text);
}
.container{max-width:1200px;margin:auto;padding:24px}

/* HERO */
.hero{
  position:relative;
  padding:64px;
  border-radius:24px;
  background:linear-gradient(180deg,rgba(255,255,255,.1),rgba(255,255,255,.03));
  overflow:hidden;
  transform-style:preserve-3d;
}
.hero h1{font-size:56px;margin:12px 0}
.hero p{max-width:620px;color:var(--muted)}
.flag{
  position:absolute;
  right:-60px;
  top:-60px;
  width:320px;
  opacity:.35;
  transform:translateZ(40px);
}
.btn{
  margin-top:28px;
  display:inline-flex;
  align-items:center;
  gap:10px;
  padding:16px 24px;
  border-radius:18px;
  font-weight:900;
  background:linear-gradient(135deg,var(--accent),#7abfff);
  color:#081020;
  text-decoration:none;
}

/* GRID */
section{margin-top:64px}
.grid{
  display:grid;
  grid-template-columns:repeat(auto-fill,minmax(220px,1fr));
  gap:18px;
}
.card{
  background:linear-gradient(180deg,rgba(255,255,255,.1),rgba(255,255,255,.03));
  border-radius:18px;
  padding:16px;
}
.card img{
  width:100%;
  height:180px;
  object-fit:cover;
  border-radius:12px;
}
.amount{font-size:22px;font-weight:900;margin-top:10px}
.note{font-size:12px;color:var(--muted)}

/* TESTIMONIALS */
.testimonials{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
  gap:18px;
}
.quote{font-size:14px}

/* FOOTER */
footer{
  margin-top:72px;
  padding-top:24px;
  border-top:1px solid rgba(255,255,255,.15);
  font-size:12px;
  color:var(--muted);
}

/* WHATSAPP */
.whatsapp{
  position:fixed;
  bottom:20px;
  right:20px;
  background:#25D366;
  color:#fff;
  padding:14px 18px;
  border-radius:999px;
  font-weight:900;
  text-decoration:none;
  box-shadow:0 12px 30px rgba(0,0,0,.35);
}

/* RESPONSIVE */
@media(max-width:900px){
  .hero{padding:36px}
  .hero h1{font-size:40px}
}
</style>
</head>

<body>
<div class="container">

  <!-- HERO -->
  <div class="hero" id="hero">
    <img class="flag" src="https://upload.wikimedia.org/wikipedia/en/a/a4/Flag_of_the_United_States.svg">
    <h1>National Grant Support Initiative</h1>
    <p>
      A high-fidelity demonstration of a modern grant funding platform,
      showcasing illustrative award scenarios, recipient profiles, and
      example public feedback.
    </p>

    <a class="btn"
       href="https://wa.me/15079617851?text=Hello%20I%20am%20interested%20in%20the%20grant%20program"
       target="_blank">
      💰 Apply for the Grant via WhatsApp
    </a>
  </div>

  <!-- RECIPIENTS -->
  <section>
    <h2>Sample Grant Recipients</h2>
    <p class="note">Stock images used. Grant amounts shown are illustrative examples.</p>

    <div class="grid">
      <div class="card"><img src="https://images.unsplash.com/photo-1600880292203-757bb62b4baf"><div class="amount">$75,000</div><div class="note">Small Business Growth</div></div>
      <div class="card"><img src="https://images.unsplash.com/photo-1521737604893-d14cc237f11d"><div class="amount">$120,000</div><div class="note">Community Development</div></div>
      <div class="card"><img src="https://images.unsplash.com/photo-1543269865-cbf427effbad"><div class="amount">$95,000</div><div class="note">Education Program</div></div>
      <div class="card"><img src="https://images.unsplash.com/photo-1523958203904-cdcb402031fd"><div class="amount">$150,000</div><div class="note">Non-Profit Operations</div></div>
      <div class="card"><img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d"><div class="amount">$60,000</div><div class="note">Agriculture Support</div></div>
      <div class="card"><img src="https://images.unsplash.com/photo-1529626455594-4ff0802cfb7e"><div class="amount">$200,000</div><div class="note">Healthcare Initiative</div></div>
      <div class="card"><img src="https://images.unsplash.com/photo-1544717305-2782549b5136"><div class="amount">$85,000</div><div class="note">Startup Funding</div></div>
      <div class="card"><img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f"><div class="amount">$110,000</div><div class="note">Workforce Training</div></div>
      <div class="card"><img src="https://images.unsplash.com/photo-1520813792240-56fc4a3765a7"><div class="amount">$140,000</div><div class="note">Infrastructure Planning</div></div>
      <div class="card"><img src="https://images.unsplash.com/photo-1551836022-d5d88e9218df"><div class="amount">$55,000</div><div class="note">Local Outreach</div></div>
    </div>
  </section>

  <!-- TESTIMONIALS -->
  <section>
    <h2>Illustrative Public Feedback</h2>
    <p class="note">Example testimonials inspired by common social-media responses.</p>

    <div class="testimonials">
      <div class="card"><div class="quote">“The grant process explanation was very clear and easy to follow.”</div><div class="note">— Sample Facebook Comment</div></div>
      <div class="card"><div class="quote">“Professional presentation and transparent eligibility requirements.”</div><div class="note">— Sample LinkedIn Post</div></div>
      <div class="card"><div class="quote">“This platform makes funding opportunities easier to understand.”</div><div class="note">— Sample Social Media Reply</div></div>
    </div>
  </section>

  <footer>
    <strong>Disclosure:</strong>
    This website is a design and development demonstration only.
    All grant amounts, images, and testimonials are illustrative and do not
    represent real recipients or an active government program.
  </footer>

</div>

<!-- FLOATING WHATSAPP -->
<a class="whatsapp"
   href="https://wa.me/15079617851?text=Hello%20I%20am%20interested%20in%20the%20grant%20program"
   target="_blank">
  💬 WhatsApp
</a>

<script>
/* Simple 4D parallax */
const hero = document.getElementById('hero');
hero.addEventListener('mousemove', e=>{
  const r = hero.getBoundingClientRect();
  const x = (e.clientX - r.left)/r.width - .5;
  const y = (e.clientY - r.top)/r.height - .5;
  hero.style.transform = `rotateX(${y*6}deg) rotateY(${x*6}deg)`;
});
hero.addEventListener('mouseleave', ()=>{
  hero.style.transform = 'rotateX(0) rotateY(0)';
});
</script>

</body>
</html>
