<!DOCTYPE html>
<html lang="en"><head><meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>For Ammu ❤️</title>
<style>
:root{--ink:#080305;--red-deep:#8b0000;--red:#e10600;--red-hot:#ff2d2d;--soft:#ffd6d6;--cream:#fff0f0}
*{box-sizing:border-box;-webkit-tap-highlight-color:transparent}
html,body{margin:0;height:100%;background:var(--ink);color:var(--cream);font-family:system-ui,-apple-system,'Segoe UI',sans-serif;overflow:hidden}
body{background:radial-gradient(900px 600px at 15% 10%,rgba(225,6,0,.28),transparent 60%),radial-gradient(800px 600px at 90% 95%,rgba(139,0,0,.45),transparent 60%),var(--ink)}
h1,h2,h3{font-family:'Brush Script MT','Pacifico',cursive;font-weight:400;margin:0}
#hearts{position:fixed;inset:0;z-index:1;pointer-events:none;overflow:hidden}
.fheart{position:absolute;bottom:-50px;opacity:0;animation:up linear forwards;filter:drop-shadow(0 0 6px rgba(255,45,45,.6))}
@keyframes up{0%{transform:translate(0,0) rotate(-12deg);opacity:0}10%{opacity:.85}90%{opacity:.85}100%{transform:translate(var(--d),-115vh) rotate(14deg);opacity:0}}
.page{position:fixed;inset:0;z-index:2;display:none;overflow-y:auto;overflow-x:hidden;padding:calc(28px + env(safe-area-inset-top,0px)) 16px calc(28px + env(safe-area-inset-bottom,0px))}
.page.active{display:flex;animation:pin .7s ease both}
@keyframes pin{from{opacity:0;transform:scale(.97)}to{opacity:1;transform:none}}
.wrap{margin:auto;width:100%;max-width:520px;text-align:center}
.card{background:rgba(25,3,6,.78);border:1.5px solid rgba(225,6,0,.6);border-radius:32px;padding:28px 22px;box-shadow:0 0 0 6px rgba(225,6,0,.08),0 18px 60px rgba(225,6,0,.28)}
.dots{position:fixed;top:calc(10px + env(safe-area-inset-top,0px));left:0;right:0;z-index:5;display:flex;justify-content:center;gap:8px;pointer-events:none}
.dots i{width:9px;height:9px;border-radius:50%;background:rgba(255,214,214,.25);transition:.4s}
.dots i.on{background:var(--red-hot);box-shadow:0 0 10px var(--red-hot);transform:scale(1.25)}
.btn{font:inherit;font-weight:700;color:#fff;border:0;cursor:pointer;border-radius:999px;padding:.85rem 1.9rem;font-size:1.1rem;background:linear-gradient(135deg,var(--red-hot),var(--red-deep));box-shadow:0 8px 24px rgba(225,6,0,.5),inset 0 1px 0 rgba(255,255,255,.3);transition:transform .15s}
.btn:active{transform:scale(.97)}
.btn:disabled{opacity:.6}
.btn.ghost{background:transparent;color:var(--soft);border:2px solid rgba(255,214,214,.5);box-shadow:none}
.btn.pulse{animation:pl 1.6s ease-in-out infinite}
@keyframes pl{0%,100%{box-shadow:0 8px 24px rgba(225,6,0,.5),0 0 0 0 rgba(255,45,45,.6)}50%{box-shadow:0 8px 24px rgba(225,6,0,.5),0 0 0 16px rgba(255,45,45,0)}}
.pets{font-size:3.4rem;line-height:1}.bounce{display:inline-block;animation:bn 2.2s ease-in-out infinite}.bounce+.bounce{animation-delay:.5s}
@keyframes bn{0%,100%{transform:translateY(0) rotate(-3deg)}50%{transform:translateY(-10px) rotate(3deg)}}
#p1 h1{font-size:clamp(2.6rem,12vw,4.4rem);line-height:1.15;color:#fff;text-shadow:0 0 18px rgba(255,45,45,.9),0 0 42px rgba(225,6,0,.6);margin:6px 0 10px}
#p1 .lead{font-size:1.12rem;line-height:1.7;color:var(--soft);margin:0 0 6px}
#p1 .ask{font-weight:700;font-size:1.2rem;margin:20px 0 16px}
#choices{display:flex;flex-direction:column;align-items:center;gap:14px;min-height:80px}
#proceed{max-width:100%;transition:all .35s cubic-bezier(.3,1.6,.5,1)}#no{transition:all .35s}
#nomsg{min-height:1.5em;margin-top:14px;color:var(--soft);font-weight:600}
h2{font-size:clamp(1.8rem,7vw,2.4rem);color:#fff;text-shadow:0 0 16px rgba(255,45,45,.85)}
.sub{color:var(--soft);margin:6px 0 14px;line-height:1.5}
.meter{height:16px;border-radius:99px;background:rgba(255,255,255,.08);border:1.5px solid rgba(225,6,0,.6);overflow:hidden;margin:0 auto 12px}
.meter b{display:block;height:100%;width:0;border-radius:99px;transition:width .3s;background:linear-gradient(90deg,var(--red-deep),var(--red-hot),#ff9a9a)}
#meterLabel{font-size:.9rem;color:var(--soft);margin:0 0 6px;font-weight:600}
#arena{position:relative;width:100%;height:min(58vh,430px);min-height:330px;overflow:hidden;touch-action:none;border-radius:26px;border:2px solid rgba(225,6,0,.65);user-select:none;-webkit-user-select:none;background:radial-gradient(circle at 50% 110%,rgba(225,6,0,.35),transparent 55%),linear-gradient(#0d0204,#2a0508)}
#arena::after{content:"";position:absolute;left:0;right:0;bottom:0;height:10px;background:repeating-linear-gradient(90deg,var(--red) 0 14px,#111 14px 28px)}
#pet{position:absolute;left:0;bottom:10px;font-size:64px;line-height:1;z-index:3;will-change:transform;filter:drop-shadow(0 4px 8px rgba(0,0,0,.7))}
#pet span{display:block}#pet.hop span{animation:hp .3s}
@keyframes hp{40%{transform:scale(1.15,.9) translateY(-6px)}}
#bubble{position:absolute;bottom:84px;left:0;z-index:4;background:#fff;color:var(--red-deep);font-weight:700;padding:4px 12px;border-radius:14px;font-size:.95rem;white-space:nowrap;opacity:0;transition:opacity .2s;pointer-events:none}
.item{position:absolute;left:0;top:0;font-size:30px;line-height:1;z-index:2;pointer-events:none}
.overlay{position:absolute;inset:0;z-index:6;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:10px;padding:20px;background:rgba(8,3,5,.9)}
.overlay h3{font-size:1.8rem;color:#fff;text-shadow:0 0 14px rgba(255,45,45,.85)}
.overlay p{margin:0 0 6px;color:var(--soft);line-height:1.6;max-width:320px}
.pick{display:flex;gap:10px}.pick .btn{padding:.6rem 1.2rem;font-size:1rem}.pick .btn.sel{background:linear-gradient(135deg,var(--red-hot),var(--red-deep));color:#fff;border-color:transparent}
.hidden{display:none!important}
.q{text-align:left;margin-bottom:18px}.q label{display:block;font-weight:700;line-height:1.5;margin-bottom:8px}.q label span{color:var(--red-hot);margin-right:6px}
textarea{width:100%;min-height:84px;resize:vertical;font:inherit;color:var(--cream);background:rgba(255,255,255,.06);border:1.5px solid rgba(225,6,0,.6);border-radius:18px;padding:12px 14px}
textarea::placeholder{color:rgba(255,214,214,.5)}textarea:focus{outline:none;border-color:var(--red-hot);box-shadow:0 0 0 4px rgba(255,45,45,.22)}
#formmsg{min-height:1.4em;color:var(--soft);font-weight:600;margin:0 0 12px}
#p4 .wrap{max-width:560px}#p4 h2{margin:6px 0 4px}#p4 .sub{margin:0 0 22px}
.stanza{background:rgba(25,3,6,.55);border:1.5px solid rgba(225,6,0,.4);border-radius:24px;padding:20px 22px;margin:0 0 16px;line-height:1.95;font-size:1.08rem;text-shadow:0 1px 8px #000;opacity:0;transform:translateY(22px);transition:opacity .9s,transform .9s}
.stanza.in{opacity:1;transform:none}.stanza.solo{border-color:rgba(255,45,45,.7);background:rgba(90,5,10,.55)}
.end{margin:26px 0 8px;font-family:'Brush Script MT',cursive;font-size:1.5rem;color:var(--soft);text-shadow:0 0 14px rgba(255,45,45,.7)}
@media (prefers-reduced-motion:reduce){.fheart,.bounce,.btn.pulse{animation:none}.fheart{opacity:.5}.stanza{transition:none;opacity:1;transform:none}}
</style></head><body>
<div id="hearts"></div>
<div class="dots"><i class="on"></i><i></i><i></i><i></i></div>

<section class="page active" id="p1"><div class="wrap"><div class="card">
<div class="pets"><span class="bounce">🐕</span> <span class="bounce">🦁</span></div>
<h1>HEY AMMU</h1>
<p class="lead">Welcome to your very own website,<br>made for you to admire yourself ✨</p>
<p class="ask">Ready to step inside?</p>
<div id="choices"><button class="btn pulse" id="proceed">Proceed ❤️</button><button class="btn ghost" id="no">No</button></div>
<div id="nomsg"></div></div></div></section>

<section class="page" id="p2"><div class="wrap"><div class="card">
<h2>Heart Catch 🐕🦁</h2>
<p class="sub">Slide your pet left and right to catch the falling love.</p>
<div class="meter"><b id="meterFill"></b></div>
<p id="meterLabel">Love meter: 0 / 12</p>
<div id="arena">
<div id="bubble">Woof!</div>
<div id="pet"><span id="petEmoji">🦁</span></div>
<div class="overlay" id="startOverlay">
<h3>Pick your pet</h3>
<div class="pick"><button class="btn ghost" data-p="🐕">🐕 Dog</button><button class="btn ghost sel" data-p="🦁">🦁 Lion</button></div>
<p>Catch 12 hearts to fill the love meter. Roses count double 🌹</p>
<button class="btn" id="startBtn">Let's play 🐾</button></div>
<div class="overlay hidden" id="winOverlay">
<div class="pets"><span class="bounce">🐕</span> <span class="bounce">🦁</span></div>
<h3>You did it! ❤️</h3>
<p>The whole pack is happy. You caught every heart like it was made for you.</p>
<button class="btn pulse" id="toP3">Ready for your surprise? 🎁</button></div>
</div></div></div></section>

<section class="page" id="p3"><div class="wrap"><div class="card">
<h2>A few little questions 💭</h2>
<p class="sub">Take your time. Answer from the heart 🖤</p>
<div class="q"><label for="q1"><span>1.</span>Would you love me as much as I do?</label><textarea id="q1" placeholder="Tell me honestly…"></textarea></div>
<div class="q"><label for="q2"><span>2.</span>What would you wanna do (what's your intention with me)?</label><textarea id="q2" placeholder="Your heart, your answer…"></textarea></div>
<div class="q"><label for="q3"><span>3.</span>To spice things up when we are together, what do you wanna do?</label><textarea id="q3" placeholder="Be bold…"></textarea></div>
<div id="formmsg" aria-live="polite"></div>
<button class="btn pulse" id="sendBtn">Here's your surprise 💌</button>
</div></div></section>

<section class="page" id="p4"><div class="wrap">
<h2>For you, Ammu</h2><p class="sub">Read it slowly 🌹</p>
<div class="stanza">Your eyes hold stories I could never fully know,<br>Beautiful like stars with a quiet glow.<br>And when you smile, the whole world feels bright,<br>Like the morning sun breaking through the night.</div>
<div class="stanza">I know someone left and shattered your heart,<br>Left you wondering why love fell apart.<br>But you don’t have to hide those tears anymore,<br>You don’t have to carry that pain like before.</div>
<div class="stanza">I’m not here to erase what happened in your past,<br>Or promise that every wound will heal fast.<br>I’m just here, with a heart that’s true,<br>Ready to be patient and gentle with you.</div>
<div class="stanza">So if your heart is scared to love again,<br>I’ll understand I won’t force you to pretend.<br>I’ll stay beside you through every scar,<br>And remind you how beautiful you are.</div>
<div class="stanza">Your eyes deserve to sparkle, not cry,<br>Your smile deserves to reach the sky.<br>And if you let me, I’ll walk by your side,<br>Until the pain fades and you feel alive.</div>
<div class="stanza solo">I can’t change the past or undo what he’s done,<br>But I can give you a reason to believe love isn’t always meant to run.</div>
<div class="stanza">So take your time, you don’t have to rush<br>I’ll be here, with patience, care, and trust.<br>Not to replace him, not to own your heart,<br>Just to show you that healing can be a beautiful start.</div>
<div class="end">…and maybe this is just the beginning ❤️</div>
</div></section>

<script>
(function(){"use strict";
var $=function(s){return document.querySelector(s)},pick=function(a){return a[Math.floor(Math.random()a.length)]},rand=function(a,b){return a+Math.random()(b-a)};
var pages=[null,$("#p1"),$("#p2"),$("#p3"),$("#p4")],dots=document.querySelectorAll(".dots i"),current=1;
function go(n){current=n;for(var i=1;i<=4;i++)pages[i].classList.toggle("active",i===n);for(var d=0;d<dots.length;d++)dots[d].classList.toggle("on",d===n-1);pages[n].scrollTop=0;if(n===4)revealStanzas()}
var layer=$("#hearts"),glyphs=["❤️","🖤","💖","❤️‍🔥","🦁","🐕"];
function spawnHeart(){if(layer.children.length>40)return;var h=document.createElement("span"),big=current===4;h.className="fheart";h.textContent=pick(glyphs);h.style.left=rand(2,96)+"%";h.style.fontSize=(big?rand(24,36):rand(13,22))+"px";h.style.setProperty("--d",rand(-60,60)+"px");h.style.animationDuration=rand(big?6:7,big?10:12)+"s";layer.appendChild(h);h.addEventListener("animationend",function(){h.remove()})}
setInterval(function(){spawnHeart();if(current===4)spawnHeart()},650);
for(var k=0;k<6;k++)setTimeout(spawnHeart,k*250);

var proceed=$("#proceed"),no=$("#no"),nomsg=$("#nomsg"),noCount=0,noLines=["Are you sure? 🥺","The lion is looking at you with sad eyes 🦁","Even the dog is begging 🐕","The Proceed button is getting bigger… 👀","Last chance for No 😏"];
no.addEventListener("click",function(){var n=++noCount;proceed.classList.remove("pulse");proceed.style.fontSize=(1.1+n*.3)+"rem";proceed.style.padding=(.85+n*.4)+"rem "+(1.9+n*.6)+"rem";proceed.style.minWidth=Math.min(n*18,96)+"%";
if(n>=5){no.style.display="none";nomsg.textContent="Oops… No ran away. Looks like there's only one button left 😘"}else{no.style.transform="scale("+(1-n*.14)+")";no.style.opacity=String(1-n*.12);nomsg.textContent=noLines[n-1]}});
proceed.addEventListener("click",function(){go(2)});

var arena=$("#arena"),pet=$("#pet"),petEmoji=$("#petEmoji"),bubble=$("#bubble"),startOverlay=$("#startOverlay"),winOverlay=$("#winOverlay"),meterFill=$("#meterFill"),meterLabel=$("#meterLabel");
var GOAL=12,score=0,running=false,items=[],px=0,lastT=0,spawnT=0,raf=0,bTO,drops=["❤️","❤️","💖","💖","🖤","💕","🦴","🌹"];
document.querySelectorAll(".pick .btn").forEach(function(b){b.addEventListener("click",function(){document.querySelectorAll(".pick .btn").forEach(function(x){x.classList.remove("sel")});b.classList.add("sel");petEmoji.textContent=b.dataset.p})});
function setPx(x,c){var w=arena.clientWidth,pw=pet.offsetWidth;px=c?x-pw/2:x;px=Math.max(0,Math.min(w-pw,px));pet.style.transform="translateX("+px+"px)"}
function center(){setPx(arena.clientWidth/2,true)}
window.addEventListener("resize",function(){setPx(px)});
function onP(e){var r=arena.getBoundingClientRect();setPx(e.clientX-r.left,true)}
arena.addEventListener("pointermove",onP);arena.addEventListener("pointerdown",onP);
window.addEventListener("keydown",function(e){if(current!==2)return;if(e.key==="ArrowLeft")setPx(px-40);if(e.key==="ArrowRight")setPx(px+40)});
function say(t){bubble.textContent=t;bubble.style.transform="translateX("+Math.max(0,px+pet.offsetWidth/2-bubble.offsetWidth/2)+"px)";bubble.style.opacity=1;clearTimeout(bTO);bTO=setTimeout(function(){bubble.style.opacity=0},650)}
function spawnItem(){var el=document.createElement("div"),g=pick(drops),x=rand(4,arena.clientWidth-40);el.className="item";el.textContent=g;el.style.transform="translate("+x+"px,-40px)";arena.appendChild(el);items.push({el:el,x:x,y:-40,v:g==="🌹"?2:1,s:rand(.9,1.25)})}
function updateMeter(){meterFill.style.width=Math.min(100,score/GOAL*100)+"%";meterLabel.textContent="Love meter: "+Math.min(score,GOAL)+" / "+GOAL}
function clear(){items.forEach(function(it){it.el.remove()});items=[]}
function loop(t){if(!running)return;var dt=Math.min((t-lastT)/16.67,3);lastT=t;spawnT+=dt*16.67;if(spawnT>Math.max(420,780-score*22)){spawnT=0;spawnItem()}
var H=arena.clientHeight,pw=pet.offsetWidth,ph=pet.offsetHeight,top=H-ph-10,sp=2.4+score*.09;
for(var i=items.length-1;i>=0;i--){var it=items[i];it.y+=sp*it.s*dt;it.el.style.transform="translate("+it.x+"px,"+it.y+"px)";var cx=it.x+15,cy=it.y+15;
if(cy>=top+10&&cy<=top+ph&&cx>=px+8&&cx<=px+pw-8){score+=it.v;it.el.remove();items.splice(i,1);pet.classList.remove("hop");void pet.offsetWidth;pet.classList.add("hop");say(pick(["Woof! ❤️","Roar! 🔥","Yay! 🐾","Yum! 😍","More! 🖤"]));updateMeter();if(score>=GOAL){win();return}}
else if(it.y>H){it.el.remove();items.splice(i,1)}}
raf=requestAnimationFrame(loop)}
function startGame(){score=0;updateMeter();clear();startOverlay.classList.add("hidden");winOverlay.classList.add("hidden");center();running=true;spawnT=700;lastT=performance.now();raf=requestAnimationFrame(loop)}
function win(){running=false;cancelAnimationFrame(raf);clear();for(var i=0;i<14;i++)setTimeout(spawnHeart,i*90);winOverlay.classList.remove("hidden")}
$("#startBtn").addEventListener("click",startGame);$("#toP3").addEventListener("click",function(){go(3)});
setTimeout(center,50);

var sendBtn=$("#sendBtn"),formmsg=$("#formmsg");
sendBtn.addEventListener("click",function(){var a1=$("#q1").value.trim(),a2=$("#q2").value.trim(),a3=$("#q3").value.trim();
if(!a1||!a2||!a3){formmsg.textContent="Please answer all three questions first 🥺";return}
formmsg.textContent="Wrapping up your surprise… 💌";sendBtn.disabled=true;var done=false;function next(){if(done)return;done=true;go(4)}
fetch("https://formspree.io/f/xwlplnyj",{method:"POST",headers:{"Content-Type":"application/json","Accept":"application/json"},body:JSON.stringify({_subject:"Ammu answered your website ❤️","1. Would you love me as much as I do?":a1,"2. What would you wanna do (what's your intention with me)?":a2,"3. To spice things up when we are together, what do you wanna do?":a3})}).then(next,next);setTimeout(next,4000)});
function revealStanzas(){var st=document.querySelectorAll(".stanza");if("IntersectionObserver" in window){var io=new IntersectionObserver(function(es){es.forEach(function(en){if(en.isIntersecting){en.target.classList.add("in");io.unobserve(en.target)}})},{root:pages[4],threshold:.2});st.forEach(function(s){io.observe(s)})}else st.forEach(function(s){s.classList.add("in")})}
})();
</script></body></html>
</html>
