<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<meta name="description" content="سایت رسمی علی گیم فول | Ali Game Full">
<meta name="theme-color" content="#050712">
<title>علی گیم فول | Ali Game Full</title>

<style>
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{
font-family:Tahoma,"Segoe UI",sans-serif;color:#fff;background:#050712;
min-height:100vh;overflow-x:hidden
}
body:before{
content:"";position:fixed;inset:0;z-index:-2;
background:
radial-gradient(circle at 20% 20%,rgba(0,255,255,.12),transparent 30%),
radial-gradient(circle at 80% 30%,rgba(255,0,170,.12),transparent 30%),
radial-gradient(circle at 50% 90%,rgba(80,0,255,.12),transparent 35%)
}
body:after{
content:"";position:fixed;inset:0;z-index:-1;pointer-events:none;
background:
linear-gradient(rgba(255,255,255,.02) 1px,transparent 1px),
linear-gradient(90deg,rgba(255,255,255,.02) 1px,transparent 1px);
background-size:45px 45px;
mask-image:linear-gradient(to bottom,#000,transparent)
}

/* منو */
nav{
position:fixed;top:0;left:0;right:0;z-index:100;
padding:15px 6%;display:flex;justify-content:space-between;align-items:center;
background:rgba(5,7,18,.75);backdrop-filter:blur(15px);
border-bottom:1px solid rgba(255,255,255,.08)
}
.logo{
font-size:1.35rem;font-weight:900;
text-shadow:0 0 8px #00ffff,0 0 18px #ff00cc
}
nav a{color:#ddd;text-decoration:none;margin-right:20px;transition:.3s}
nav a:hover{color:#00ffff}

/* صفحه اصلی */
.hero{
min-height:100vh;display:flex;align-items:center;justify-content:center;
text-align:center;padding:110px 20px 60px
}
.hero-card{
width:min(900px,95%);padding:55px 30px;border-radius:35px;
background:rgba(10,14,30,.75);backdrop-filter:blur(22px);
border:1px solid rgba(255,255,255,.1);
box-shadow:0 0 40px rgba(0,255,255,.08),0 30px 80px rgba(0,0,0,.5);
position:relative;overflow:hidden
}
.hero-card:before{
content:"";position:absolute;width:500px;height:500px;top:-300px;left:-150px;
background:radial-gradient(circle,rgba(0,255,255,.18),transparent 65%);
animation:float 7s ease-in-out infinite
}
.badge{
display:inline-block;padding:8px 18px;border-radius:50px;
background:rgba(0,255,255,.08);border:1px solid rgba(0,255,255,.35);
color:#00ffff;margin-bottom:22px;font-weight:bold
}
h1{
font-size:clamp(2.5rem,8vw,5.5rem);font-weight:1000;line-height:1.1;
margin-bottom:15px;background:linear-gradient(90deg,#fff,#00ffff,#ff00cc,#fff);
background-size:300%;-webkit-background-clip:text;background-clip:text;color:transparent;
animation:gradient 5s linear infinite
}
.subtitle{
color:#cbd5e1;font-size:clamp(1rem,3vw,1.35rem);
margin-bottom:35px;line-height:1.9
}

/* دکمه ها */
.buttons{
display:grid;grid-template-columns:repeat(2,1fr);
gap:14px;max-width:650px;margin:auto
}
.btn{
position:relative;overflow:hidden;display:flex;justify-content:center;align-items:center;
min-height:58px;border-radius:17px;text-decoration:none;color:#fff;
font-weight:900;border:1px solid rgba(255,255,255,.12);
transition:.3s;box-shadow:0 8px 25px rgba(0,0,0,.2)
}
.btn:hover{transform:translateY(-5px) scale(1.02);filter:brightness(1.15)}
.btn:after{
content:"";position:absolute;width:100px;height:200%;
background:rgba(255,255,255,.18);
transform:rotate(25deg) translateX(-180px);transition:.6s
}
.btn:hover:after{transform:rotate(25deg) translateX(400px)}
.donate{background:linear-gradient(135deg,#ec4899,#8b5cf6)}
.youtube{background:linear-gradient(135deg,#ff0000,#a00000)}
.aparat{background:linear-gradient(135deg,#ffb000,#f15a00)}
.rubika{background:linear-gradient(135deg,#8b5cf6,#4c1d95)}

/* بخش ها */
section{padding:80px 6%}
.section-title{text-align:center;font-size:2rem;margin-bottom:35px}
.section-title span{color:#00ffff;text-shadow:0 0 15px rgba(0,255,255,.5)}  
.cards{
max-width:1000px;margin:auto;display:grid;
grid-template-columns:repeat(3,1fr);gap:20px
}
.info-card{
padding:30px 20px;text-align:center;border-radius:25px;
background:rgba(255,255,255,.04);
border:1px solid rgba(255,255,255,.08);
backdrop-filter:blur(15px);transition:.3s
}
.info-card:hover{
transform:translateY(-8px);border-color:rgba(0,255,255,.35);
box-shadow:0 0 30px rgba(0,255,255,.08)
}
.icon{font-size:2.8rem;margin-bottom:15px}
.info-card h3{margin-bottom:10px}
.info-card p,.about p{color:#cbd5e1;line-height:2}

.about{
max-width:900px;margin:auto;text-align:center;padding:40px;
border-radius:30px;background:rgba(255,255,255,.035);
border:1px solid rgba(255,255,255,.08);backdrop-filter:blur(15px)
}
footer{
text-align:center;padding:35px 20px;color:#64748b;
border-top:1px solid rgba(255,255,255,.07)
}
footer strong{color:#00ffff}

/* انیمیشن */
@keyframes gradient{
0%{background-position:0}100%{background-position:300%}
}
@keyframes float{
0%,100%{transform:translate(0,0)}
50%{transform:translate(100px,80px)}
}
/* موبایل */
@media(max-width:700px){
nav{padding:13px 18px}
nav .links{display:none}
.hero{padding-top:90px}
.hero-card{padding:40px 18px}
.buttons,.cards{grid-template-columns:1fr}
section{padding:60px 18px}
.about{padding:25px 18px}
}
</style>
</head>

<body>

<nav>
<div class="logo">🎮 Ali Game Full</div>
<div class="links">
<a href="#home">خانه</a>
<a href="#channels">کانال‌ها</a>
<a href="#about">درباره من</a>
</div>
</nav>

<main id="home" class="hero">
<div class="hero-card">

<div class="badge">🔥 دنیای گیمینگ علی گیم فول</div>

<h1>علی گیم فول</h1>

<p class="subtitle">
Ali Game Full<br>
گیم، سرگرمی، چالش و کلی ویدیوی خفن 🎮🔥
</p>

<div class="buttons">

<a class="btn donate" href="https://Reymit.ir/ali.game.full" target="_blank" rel="noopener noreferrer">
💜 حمایت مالی
</a>

<a class="btn youtube" href="https://www.youtube.com/@Ali.Game.Full1" target="_blank" rel="noopener noreferrer">
▶️ کانال یوتیوب
</a>

<a class="btn aparat" href="https://www.aparat.com/Ali.Game.Full" target="_blank" rel="noopener noreferrer">
🎬 کانال آپارات
</a>

<a class="btn rubika" href="https://rubika.ir/Ali_Game_Full" target="_blank" rel="noopener noreferrer">
💬 کانال روبیکا
</a>

</div>
</div>
</main>

<section id="channels">

<h2 class="section-title">
چرا <span>علی گیم فول؟</span>
</h2>

<div class="cards">

<div class="info-card">
<div class="icon">🎮</div>
<h3>گیمینگ</h3>
<p>ویدیوهای گیمینگ، چالش‌ها و لحظات جذاب از بازی‌های مختلف.</p>
</div>

<div class="info-card">
<div class="icon">🔥</div>
<h3>محتوای جدید</h3>
<p>ویدیوها و سرگرمی‌های جدید را در کانال‌های علی گیم فول دنبال کنید.</p>
</div>

<div class="info-card">
<div class="icon">🚀</div>
<h3>حمایت شما</h3>
<p>حمایت شما باعث می‌شود محتوای بیشتر و حرفه‌ای‌تری تولید کنیم.</p>
</div>

</div>
</section>

<section id="about">

<h2 class="section-title">
درباره <span>علی گیم فول</span>
</h2>

<div class="about">
<p>
به سایت رسمی علی گیم فول خوش آمدید! 🎮
<br><br>
اینجا می‌توانید به شبکه‌های اجتماعی و کانال‌های من دسترسی داشته باشید
و جدیدترین ویدیوها و فعالیت‌های گیمینگ را دنبال کنید.
<br><br>
ممنون که از علی گیم فول حمایت می‌کنید ❤️🔥
</p>
</div>

</section>

<footer>
<strong>Ali Game Full</strong> © 2026
</footer>

</body>
</html>
