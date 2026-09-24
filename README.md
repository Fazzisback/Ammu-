<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>For Ammu 💕</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Quicksand:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
  :root{
    --ink:#1a0812;
    --pink-deep:#a3195b;
    --pink:#ff4d94;
    --pink-hot:#ff6fb0;
    --rose:#ffd1e6;
    --cream:#fff0f6;
  }
  *{box-sizing:border-box;-webkit-tap-highlight-color:transparent}
  html,body{margin:0;height:100%;background:var(--ink);color:var(--cream);
    font-family:'Quicksand',system-ui,-apple-system,'Segoe UI',sans-serif;overflow:hidden}
  body{
    background:
      radial-gradient(900px 600px at 15% 10%, rgba(255,77,148,.30), transparent 60%),
      radial-gradient(800px 600px at 90% 95%, rgba(163,25,91,.38), transparent 60%),
      var(--ink);
  }
  h1,h2{font-family:'Pacifico','Brush Script MT',cursive;font-weight:400;margin:0}

  #hearts{position:fixed;inset:0;z-index:1;pointer-events:none;overflow:hidden}
  .fheart{position:absolute;bottom:-50px;opacity:0;animation:floatUp linear forwards;
    filter:drop-shadow(0 0 6px rgba(255,111,176,.55))}
  @keyframes floatUp{
    0%{transform:translate(0,0) rotate(-12deg);opacity:0}
    10%{opacity:.85}
    90%{opacity:.85}
    100%{transform:translate(var(--drift),-115vh) rotate(14deg);opacity:0}
  }

  .page{position:fixed;inset:0;z-index:2;display:none;overflow-y:auto;overflow-x:hidden;
    padding:calc(28px + env(safe-area-inset-top,0px)) 16px calc(28px + env(safe-area-inset-bottom,0px))}
  .page.active{display:flex;animation:pageIn .7s ease both}
  @keyframes pageIn{from{opacity:0;transform:scale(.97)}to{opacity:1;transform:none}}
  .wrap{margin:auto;width:100%;max-width:520px;text-align:center}

  .card{background:rgba(50,8,28,.72);border:1.5px solid rgba(255,111,176,.5);border-radius:32px;
    padding:28px 22px;box-shadow:0 0 0 6px rgba(255,77,148,.08),0 18px 60px rgba(255,77,148,.25);
    backdrop-filter:blur(6px);-webkit-backdrop-filter:blur(6px)}

  .dots{position:fixed;top:calc(10px + env(safe-area-inset-top,0px));left:0;right:0;z-index:5;
    display:flex;justify-content:center;gap:8px;pointer-events:none}
  .dots i{width:9px;height:9px;border-radius:50%;background:rgba(255,209,230,.25);transition:.4s}
  .dots i.on{background:var(--pink-hot);box-shadow:0 0 10px var(--pink-hot);transform:scale(1.25)}

  .btn{font:inherit;font-weight:700;color:#fff;border:0;cursor:pointer;border-radius:999px;
    padding:.85rem 1.9rem;font-size:1.1rem;
    background:linear-gradient(135deg,var(--pink-hot),var(--pink-deep));
    box-shadow:0 8px 24px rgba(255,77,148,.45),inset 0 1px 0 rgba(255,255,255,.35);
    transition:transform .15s ease,box-shadow .15s ease}
  .btn:hover{transform:translateY(-2px) scale(1.03)}
  .btn:active{transform:scale(.97)}
  .btn:focus-visible,textarea:focus-visible{outline:3px solid var(--rose);outline-offset:3px}
  .btn.ghost{background:transparent;color:var(--rose);border:2px solid rgba(255,209,230,.6);box-shadow:none}
  .btn.pulse{animation:pulse 1.6s ease-in-out infinite}
  @keyframes pulse{0%,100%{box-shadow:0 8px 24px rgba(255,77,148,.45),0 0 0 0 rgba(255,111,176,.6)}
                   50%{box-shadow:0 8px 24px rgba(255,77,148,.45),0 0 0 16px rgba(255,111,176,0)}}

  .poodle-svg{display:block;margin:0 auto}
  .bounce{animation:bounce 2.2s ease-in-out infinite}
  @keyframes bounce{0%,100%{transform:translateY(0) rotate(-3deg)}50%{transform:translateY(-10px) rotate(3deg)}}

  #p1 h1{font-size:clamp(2.6rem,12vw,4.4rem);line-height:1.15;color:#fff;
    text-shadow:0 0 18px rgba(255,111,176,.85),0 0 42px rgba(255,77,148,.6);margin:6px 0 10px}
  #p1 .lead{font-size:1.12rem;line-height:1.7;color:var(--rose);margin:0 0 6px}
  #p1 .ask{font-weight:700;font-size:1.2rem;margin:20px 0 16px}
  #choices{display:flex;flex-direction:column;align-items:center;gap:14px;min-height:80px}
  #proceed{max-width:100%;transition:all .35s cubic-bezier(.3,1.6,.5,1)}
  #no{transition:all .35s ease}
  #nomsg{min-height:1.5em;margin-top:14px;color:var(--rose);font-weight:600}

  #p2 h2{font-size:clamp(1.8rem,7vw,2.4rem);color:#fff;text-shadow:0 0 16px rgba(255,111,176,.8)}
  #p2 .sub{color:var(--rose);margin:6px 0 14px;line-height:1.5}
  .meter{height:16px;border-radius:99px;background:rgba(255,255,255,.08);border:1.5px solid rgba(255,111,176,.55);
    overflow:hidden;margin:0 auto 12px;position:relative}
  .meter b{display:block;height:100%;width:0;border-radius:99px;transition:width .3s ease;
    background:linear-gradient(90deg,var(--pink-deep),var(--pink-hot),#ffc2de)}
  .meter-label{font-size:.9rem;color:var(--rose);margin:0 0 6px;font-weight:600}
  #arena{position:relative;width:100%;height:min(58vh,430px);min-height:330px;overflow:hidden;touch-action:none;
    border-radius:26px;border:2px solid rgba(255,111,176,.6);user-select:none;-webkit-user-select:none;
    background:
      radial-gradient(circle at 50% 110%, rgba(255,111,176,.35), transparent 55%),
      linear-gradient(#22091a,#3d0e2b);
    box-shadow:inset 0 0 40px rgba(0,0,0,.6),0 0 30px rgba(255,77,148,.25)}
  #arena::after{content:"";position:absolute;left:0;right:0;bottom:0;height:10px;
    background:repeating-linear-gradient(90deg,var(--pink-deep) 0 14px,#6e1140 14px 28px)}
  #poodle{position:absolute;left:0;bottom:8px;width:92px;will-change:transform;z-index:3}
  #poodle svg{width:100%;height:auto;display:block;filter:drop-shadow(0 4px 8px rgba(0,0,0,.6))}
  #poodle.hop svg{animation:hop .3s ease}
  @keyframes hop{0%{transform:scale(1)}40%{transform:scale(1.15,.9) translateY(-6px)}100%{transform:scale(1)}}
  #bubble{position:absolute;bottom:104px;left:0;z-index:4;background:#fff;color:var(--pink-deep);font-weight:700;
    padding:4px 12px;border-radius:14px;font-size:.95rem;white-space:nowrap;opacity:0;transition:opacity .2s;pointer-events:none}
  #bubble::after{content:"";position:absolute;left:50%;bottom:-6px;margin-left:-6px;border:6px solid transparent;
    border-top-color:#fff;border-bottom:0}
  .item{position:absolute;left:0;top:0;font-size:30px;line-height:1;will-change:transform;z-index:2;pointer-events:none}
  .overlay{position:absolute;inset:0;z-index:6;display:flex;flex-direction:column;align-items:center;justify-content:center;
    gap:10px;padding:20px;background:rgba(26,8,18,.88);backdrop-filter:blur(3px)}
  .overlay h3{font-family:'Pacifico',cursive;font-weight:400;font-size:1.7rem;margin:0;color:#fff;text-shadow:0 0 14px rgba(255,111,176,.8)}
  .overlay p{margin:0 0 6px;color:var(--rose);line-height:1.6;max-width:320px}
  .hidden{display:none !important}

  #p3 h2{font-size:clamp(1.8rem,7vw,2.3rem);color:#fff;text-shadow:0 0 16px rgba(255,111,176,.8)}
  #p3 .sub{color:var(--rose);margin:6px 0 20px}
  .q{text-align:left;margin-bottom:18px}
  .q label{display:block;font-weight:700;line-height:1.5;margin-bottom:8px}
  .q label span{color:var(--pink-hot);margin-right:6px}
  textarea{width:100%;min-height:84px;resize:vertical;font:inherit;color:var(--cream);
    background:rgba(255,255,255,.06);border:1.5px solid rgba(255,111,176,.55);border-radius:18px;padding:12px 14px;
    transition:box-shadow .2s,border-color .2s}
  textarea::placeholder{color:rgba(255,209,230,.5)}
  textarea:focus{outline:none;border-color:var(--pink-hot);box-shadow:0 0 0 4px rgba(255,111,176,.22)}
  #formmsg{min-height:1.4em;color:var(--rose);font-weight:600;margin:0 0 12px}

  #p4 .wrap{max-width:560px}
  #p4 h2{font-size:clamp(2rem,8vw,2.8rem);color:#fff;text-shadow:0 0 18px rgba(255,111,176,.9),0 0 40px rgba(255,77,148,.6);margin:6px 0 4px}
  #p4 .sub{color:var(--rose);margin:0 0 22px}
  .stanza{background:rgba(46,8,26,.42);border:1.5px solid rgba(255,111,176,.35);border-radius:24px;
    padding:20px 22px;margin:0 0 16px;line-height:1.95;font-size:1.08rem;font-weight:500;
    text-shadow:0 1px 8px rgba(0,0,0,.9);
    opacity:0;transform:translateY(22px);transition:opacity .9s ease,transform .9s ease}
  .stanza.in{opacity:1;transform:none}
  .stanza.solo{border-color:rgba(255,111,176,.6);background:rgba(90,10,52,.5)}
  .end{margin:26px 0 8px;font-family:'Pacifico',cursive;font-size:1.4rem;color:var(--rose);text-shadow:0 0 14px rgba(255,111,176,.7)}

  @media (prefers-reduced-motion:reduce){
    .fheart,.bounce,.btn.pulse{animation:none}
    .fheart{opacity:.5}
    .stanza{transition:none;opacity:1;transform:none}
  }
</style>
</head>
<body data-page="1">

<svg width="0" height="0" style="position:absolute" aria-hidden="true">
  <defs>
    <symbol id="poodle-art" viewBox="0 0 120 124">
      <g fill="#fff4ec" stroke="#f0cfc4" stroke-width="1.2">
        <circle cx="24" cy="66" r="18"/><circle cx="17" cy="84" r="14"/><circle cx="12" cy="70" r="9"/>
        <circle cx="96" cy="66" r="18"/><circle cx="103" cy="84" r="14"/><circle cx="108" cy="70" r="9"/>
        <circle cx="60" cy="22" r="17"/><circle cx="43" cy="30" r="14"/><circle cx="77" cy="30" r="14"/>
        <ellipse cx="60" cy="72" rx="35" ry="33"/>
      </g>
      <ellipse cx="60" cy="87" rx="17" ry="13" fill="#ffffff"/>
      <ellipse cx="41" cy="80" rx="7" ry="4" fill="#ff8fa8" opacity=".55"/>
      <ellipse cx="79" cy="80" rx="7" ry="4" fill="#ff8fa8" opacity=".55"/>
      <circle cx="46" cy="68" r="5.6" fill="#1a0a0d"/><circle cx="74" cy="68" r="5.6" fill="#1a0a0d"/>
      <circle cx="47.8" cy="66" r="2" fill="#fff"/><circle cx="75.8" cy="66" r="2" fill="#fff"/>
      <ellipse cx="60" cy="81" rx="6.5" ry="4.8" fill="#1a0a0d"/>
      <ellipse cx="58.2" cy="79.6" rx="2" ry="1.2" fill="#fff" opacity=".8"/>
      <path d="M60 85.5v4M60 89.5q-6 6-11 1M60 89.5q6 6 11 1" fill="none" stroke="#1a0a0d" stroke-width="2" stroke-linecap="round"/>
      <path d="M55.5 93q4.5 10 9 0z" fill="#ff5c7c"/>
      <path d="M60 40L42 30v20z" fill="#ff4d94"/><path d="M60 40l18-10v20z" fill="#ff4d94"/>
      <circle cx="60" cy="40" r="5.5" fill="#a3195b"/>
    </symbol>
  </defs>
</svg>

<div id="hearts" aria-hidden="true"></div>
<div class="dots" aria-hidden="true"><i class="on"></i><i></i><i></i><i></i></div>

<!-- ================= PAGE 1 ================= -->
<section class="page active" id="p1">
  <div class="wrap card">
    <svg class="poodle-svg bounce" width="130" height="134" viewBox="0 0 120 124" role="img" aria-label="Cute poodle"><use href="#poodle-art"/></svg>
    <h1>HEY AMMU</h1>
    <p class="lead">Welcome to your very own website,<br>made for you to admire yourself ✨</p>
    <p class="ask">Ready to step inside?</p>
    <div id="choices">
      <button class="btn pulse" id="proceed">Proceed 💖</button>
      <button class="btn ghost" id="no">No</button>
    </div>
    <div id="nomsg" aria-live="polite"></div>
  </div>
</section>

<!-- ================= PAGE 2 ================= -->
<section class="page" id="p2">
  <div class="wrap">
    <h2>Coco's Heart Catch 🐩</h2>
    <p class="sub">Slide Coco left and right to catch the falling love.</p>
    <p class="meter-label" id="meterLabel">Love meter: 0 / 12</p>
    <div class="meter"><b id="meterFill"></b></div>

    <div id="arena">
      <div id="bubble">Woof!</div>
      <div id="poodle"><svg viewBox="0 0 120 124"><use href="#poodle-art"/></svg></div>

      <div class="overlay" id="startOverlay">
        <svg class="poodle-svg bounce" width="96" height="100" viewBox="0 0 120 124"><use href="#poodle-art"/></svg>
        <h3>Meet Coco</h3>
        <p>Coco is a little poodle who is very hungry for love. Catch 12 hearts to fill her love meter. Roses count double 🌹</p>
        <button class="btn" id="startBtn">Let's play 🐾</button>
      </div>

      <div class="overlay hidden" id="winOverlay">
        <svg class="poodle-svg bounce" width="96" height="100" viewBox="0 0 120 124"><use href="#poodle-art"/></svg>
        <h3>You did it! 💕</h3>
        <p>Coco is so happy she could do zoomies. You caught every heart like it was made for you.</p>
        <button class="btn pulse" id="toP3">Ready for your surprise? 🎁</button>
      </div>
    </div>
  </div>
</section>

<!-- ================= PAGE 3 ================= -->
<section class="page" id="p3">
  <div class="wrap card">
    <h2>A few little questions 💭</h2>
    <p class="sub">Take your time. Answer from the heart 🐾</p>

    <div class="q">
      <label for="q1"><span>1.</span>Would you love me?</label>
      <textarea id="q1" placeholder="Tell me honestly…"></textarea>
    </div>
    <div class="q">
      <label for="q2"><span>2.</span>When are we gonna meet?</label>
      <textarea id="q2" placeholder="Your heart, your answer…"></textarea>
    </div>
    <div class="q">
      <label for="q3"><span>3.</span>I'm addicted to you 💕 are you??</label>
      <textarea id="q3" placeholder="What do you think?"></textarea>
    </div>

    <div id="formmsg" aria-live="polite"></div>
    <button class="btn pulse" id="sendBtn">Here's your surprise 💌</button>
  </div>
</section>

<!-- ================= PAGE 4 ================= -->
<section class="page" id="p4">
  <div class="wrap">
    <svg class="poodle-svg bounce" width="86" height="90" viewBox="0 0 120 124"><use href="#poodle-art"/></svg>
    <h2>For you, Ammu</h2>
    <p class="sub">Read it slowly 🌹</p>

    <div class="stanza">Your eyes hold stories I could never fully know,<br>
Beautiful like stars with a quiet glow.<br>
And when you smile, the whole world feels bright,<br>
Like the morning sun breaking through the night.</div>

    <div class="stanza">I know someone left and shattered your heart,<br>
Left you wondering why love fell apart.<br>
But you don’t have to hide those tears anymore,<br>
You don’t have to carry that pain like before.</div>

    <div class="stanza">I’m not here to erase what happened in your past,<br>
Or promise that every wound will heal fast.<br>
I’m just here, with a heart that’s true,<br>
Ready to be patient and gentle with you.</div>

    <div class="stanza">So if your heart is scared to love again,<br>
I’ll understand I won’t force you to pretend.<br>
I’ll stay beside you through every scar,<br>
And remind you how beautiful you are.</div>

    <div class="stanza">Your eyes deserve to sparkle, not cry,<br>
Your smile deserves to reach the sky.<br>
And if you let me, I’ll walk by your side,<br>
Until the pain fades and you feel alive.</div>

    <div class="stanza solo">I can’t change the past or undo what he’s done,<br>
But I can give you a reason to believe love isn’t always meant to run.</div>

    <div class="stanza">So take your time, you don’t have to rush<br>
I’ll be here, with patience, care, and trust.<br>
Not to replace him, not to own your heart,<br>
Just to show you that healing can be a beautiful start.</div>

    <div class="end">…and maybe this is just the beginning 💖</div>
  </div>
</section>

<script>
(function(){
  "use strict";
  var $ = function(s){ return document.querySelector(s); };
  var pick = function(a){ return a[Math.floor(Math.random()*a.length)]; };
  var rand = function(a,b){ return a + Math.random()*(b-a); };

  var pages = [null,$("#p1"),$("#p2"),$("#p3"),$("#p4")];
  var dots = document.querySelectorAll(".dots i");
  var current = 1;
  function go(n){
    current = n;
    for(var i=1;i<=4;i++) pages[i].classList.toggle("active", i===n);
    for(var d=0; d<dots.length; d++) dots[d].classList.toggle("on", d===n-1);
    document.body.dataset.page = n;
    pages[n].scrollTop = 0;
    if(n===4) revealStanzas();
  }

  var layer = $("#hearts");
  var glyphs = ["💖","💕","💗","❤️","💘"];
  function spawnHeart(){
    if(layer.childElementCount > 40) return;
    var h = document.createElement("span");
    var big = (current === 4);
    h.className = "fheart";
    h.textContent = pick(glyphs);
    h.style.left = rand(2,96) + "%";
    h.style.fontSize = (big ? rand(24,36) : rand(13,22)) + "px";
    h.style.setProperty("--drift", rand(-60,60) + "px");
    h.style.animationDuration = rand(big?6:7, big?10:12) + "s";
    layer.appendChild(h);
    h.addEventListener("animationend", function(){ h.remove(); });
  }
  setInterval(function(){ spawnHeart(); if(current===4) spawnHeart(); }, 650);
  for(var k=0;k<6;k++) setTimeout(spawnHeart, k*250);

  var proceed = $("#proceed"), no = $("#no"), nomsg = $("#nomsg");
  var noCount = 0;
  var noLines = [
    "Are you sure? 🥺",
    "Coco is looking at you with sad eyes 🐩",
    "Pretty please? 💕",
    "The Proceed button is getting bigger… 👀",
    "Last chance for No 😏"
  ];
  no.addEventListener("click", function(){
    noCount++;
    var n = noCount;
    proceed.classList.remove("pulse");
    proceed.style.fontSize = (1.1 + n*0.3) + "rem";
    proceed.style.padding = (0.85 + n*0.4) + "rem " + (1.9 + n*0.6) + "rem";
    proceed.style.minWidth = Math.min(n*18, 96) + "%";
    if(n >= 5){
      no.style.display = "none";
      nomsg.textContent = "Oops… No ran away. Looks like there's only one button left 😘";
    } else {
      no.style.transform = "scale(" + (1 - n*0.14) + ")";
      no.style.opacity = String(1 - n*0.12);
      nomsg.textContent = noLines[n-1];
    }
  });
  proceed.addEventListener("click", function(){ go(2); });

  var arena = $("#arena"), poodle = $("#poodle"), bubble = $("#bubble");
  var startOverlay = $("#startOverlay"), winOverlay = $("#winOverlay");
  var meterFill = $("#meterFill"), meterLabel = $("#meterLabel");
  var GOAL = 12, score = 0, running = false, items = [], px = 0, lastT = 0, spawnT = 0, raf = 0, bubbleTO;
  var drops = ["💖","💖","💗","💗","❤️","💕","🦴","🌹"];

  function setPx(x, isCenter){
    var w = arena.clientWidth, pw = poodle.offsetWidth;
    px = isCenter ? x - pw/2 : x;
    px = Math.max(0, Math.min(w - pw, px));
    poodle.style.transform = "translateX(" + px + "px)";
  }
  function centerPoodle(){ setPx(arena.clientWidth/2, true); }
  centerPoodle();
  window.addEventListener("resize", function(){ setPx(px); });

  function onPointer(e){
    var r = arena.getBoundingClientRect();
    setPx(e.clientX - r.left, true);
  }
  arena.addEventListener("pointermove", onPointer);
  arena.addEventListener("pointerdown", onPointer);
  window.addEventListener("keydown", function(e){
    if(current !== 2) return;
    if(e.key === "ArrowLeft") setPx(px - 40);
    if(e.key === "ArrowRight") setPx(px + 40);
  });

  function say(text){
    bubble.textContent = text;
    bubble.style.transform = "translateX(" + (px + poodle.offsetWidth/2 - bubble.offsetWidth/2) + "px)";
    bubble.style.opacity = 1;
    clearTimeout(bubbleTO);
    bubbleTO = setTimeout(function(){ bubble.style.opacity = 0; }, 650);
  }

  function spawnItem(){
    var el = document.createElement("div");
    var glyph = pick(drops);
    el.className = "item";
    el.textContent = glyph;
    var x = rand(4, arena.clientWidth - 40);
    el.style.transform = "translate(" + x + "px,-40px)";
    arena.appendChild(el);
    items.push({el:el, x:x, y:-40, v: glyph === "🌹" ? 2 : 1, s: rand(0.9,1.25)});
  }

  function updateMeter(){
    var pct = Math.min(100, score/GOAL*100);
    meterFill.style.width = pct + "%";
    meterLabel.textContent = "Love meter: " + Math.min(score,GOAL) + " / " + GOAL;
  }

  function loop(t){
    if(!running) return;
    var dt = Math.min((t - lastT)/16.67, 3);
    lastT = t;
    spawnT += dt*16.67;
    if(spawnT > Math.max(420, 780 - score*22)){ spawnT = 0; spawnItem(); }

    var H = arena.clientHeight, pw = poodle.offsetWidth, ph = poodle.offsetHeight;
    var top = H - ph - 8;
    var speed = 2.4 + score*0.09;

    for(var i = items.length-1; i>=0; i--){
      var it = items[i];
      it.y += speed*it.s*dt;
      it.el.style.transform = "translate(" + it.x + "px," + it.y + "px)";
      var cx = it.x + 15, cy = it.y + 15;
      if(cy >= top + 14 && cy <= top + ph && cx >= px + 10 && cx <= px + pw - 10){
        score += it.v;
        it.el.remove(); items.splice(i,1);
        poodle.classList.remove("hop"); void poodle.offsetWidth; poodle.classList.add("hop");
        say(pick(["Woof! 💕","Yay! 🐾","Yum! 🥰","Arf arf! 💖","More! 😍"]));
        updateMeter();
        if(score >= GOAL){ win(); return; }
      } else if(it.y > H){
        it.el.remove(); items.splice(i,1);
      }
    }
    raf = requestAnimationFrame(loop);
  }

  function startGame(){
    score = 0; updateMeter();
    items.forEach(function(it){ it.el.remove(); }); items = [];
    startOverlay.classList.add("hidden");
    winOverlay.classList.add("hidden");
    centerPoodle();
    running = true; spawnT = 700; lastT = performance.now();
    raf = requestAnimationFrame(loop);
  }
  function win(){
    running = false; cancelAnimationFrame(raf);
    items.forEach(function(it){ it.el.remove(); }); items = [];
    for(var i=0;i<14;i++) setTimeout(spawnHeart, i*90);
    winOverlay.classList.remove("hidden");
  }
  $("#startBtn").addEventListener("click", startGame);
  $("#toP3").addEventListener("click", function(){ go(3); });

  var sendBtn = $("#sendBtn"), formmsg = $("#formmsg");
  sendBtn.addEventListener("click", function(){
    var a1 = $("#q1").value.trim(), a2 = $("#q2").value.trim(), a3 = $("#q3").value.trim();
    if(!a1 || !a2 || !a3){
      formmsg.textContent = "Please answer all three questions first 🥺";
      return;
    }
    formmsg.textContent = "Wrapping up your surprise… 💌";
    sendBtn.disabled = true;
    var done = false;
    function next(){ if(done) return; done = true; go(4); }
    fetch("https://formspree.io/f/xwlplnyj", {
      method: "POST",
      headers: {"Content-Type":"application/json","Accept":"application/json"},
      body: JSON.stringify({
        _subject: "Ammu answered your website 💕",
        "1. Would you love me?": a1,
        "2. When are we gonna meet?": a2,
        "3. I'm addicted to you, are you?": a3
      })
    }).then(next, next);
    setTimeout(next, 4000);
  });

  function revealStanzas(){
    var st = document.querySelectorAll(".stanza");
    if("IntersectionObserver" in window){
      var io = new IntersectionObserver(function(entries){
        entries.forEach(function(en){
          if(en.isIntersecting){ en.target.classList.add("in"); io.unobserve(en.target); }
        });
      }, {root: pages[4], threshold: 0.2});
      st.forEach(function(s){ io.observe(s); });
    } else {
      st.forEach(function(s){ s.classList.add("in"); });
    }
  }
})();
</script>
</body>
</html>
