<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>A little question for you ♡</title>
<style>
/* Change these colors to personalize your page. */
:root{--pink:#df678c;--ink:#9c4363;--paper:#fffaf7;--blush:#f8dfe2}
*{box-sizing:border-box}body{margin:0;min-height:100svh;display:grid;place-items:center;background:var(--paper);color:var(--ink);font-family:Georgia,'Times New Roman',serif;overflow-x:hidden}button{font:inherit;cursor:pointer}button:focus-visible{outline:3px solid #943559;outline-offset:6px}[hidden]{display:none!important}
.stage{position:relative;isolation:isolate;width:100%;min-height:80svh;display:grid;place-items:center;padding:80px 22px;background:radial-gradient(ellipse at center,#fff0ed 0%,#f5dadd 80%);border-block:3px solid #ecc0cb;box-shadow:0 0 35px #efc6ce66}
.stage:before,.stage:after{content:"";position:absolute;left:0;right:0;height:24px;background:radial-gradient(ellipse at 50% 0, var(--paper) 65%,transparent 68%) 0 0/48px 25px repeat-x;z-index:-1}.stage:before{top:-3px}.stage:after{bottom:-3px;transform:rotate(180deg)}
.speckles{position:absolute;inset:0;overflow:hidden;pointer-events:none;z-index:-1}.petal{position:absolute;left:var(--x);top:110%;color:#d7899b;opacity:0;animation:float var(--time) linear infinite;animation-delay:var(--delay);font-size:var(--size)}
@keyframes float{0%{transform:translate(0,0) rotate(0);opacity:0}15%,80%{opacity:.5}100%{transform:translate(55px,-95vh) rotate(190deg);opacity:0}}
.panel{text-align:center;width:min(100%,520px);animation:appear .65s ease both}.eyebrow{font:11px/1.6 Arial,sans-serif;letter-spacing:3px;text-transform:uppercase;color:#bd8291;margin:0 0 30px}.mascot{width:150px;height:154px;overflow:visible;animation:bob 3s ease-in-out infinite}.heart{transform-origin:center;animation:beat 1.1s ease-in-out infinite}.tiny-heart{font-size:22px;fill:#dc7996}h1{font-size:clamp(29px,6vw,43px);font-weight:normal;line-height:1.2;margin:12px 0}p{font-size:16px;line-height:1.6;margin:10px 0}.sub{color:#b17a89}.choices{position:relative;display:flex;justify-content:center;align-items:center;gap:18px;min-height:108px}.btn{border:0;border-radius:14px;padding:15px 30px;transition:transform .2s,box-shadow .2s;background:var(--pink);color:white;box-shadow:0 6px 0 #c35377,0 10px 20px #dc7c9330;font:bold 16px Arial,sans-serif}.btn:hover{transform:translateY(-3px)}.btn:active{transform:translateY(3px);box-shadow:0 2px 0 #c35377}.no{background:#fffaf6;color:#a17a82;box-shadow:0 5px 0 #e6c6ce;z-index:5}.hint{font-size:12px;color:#b88995;min-height:20px}.meter-label{font:bold 14px Arial,sans-serif;color:var(--pink)}.count{display:block;font-size:clamp(65px,16vw,95px);font-weight:bold;color:var(--pink);margin:8px}.track{height:10px;width:min(260px,80%);margin:20px auto;background:#fff7f5;border-radius:20px;overflow:hidden}.fill{height:100%;width:0;background:var(--pink);border-radius:20px}.envelope{display:block;position:relative;width:250px;height:158px;margin:42px auto 20px;background:#eeb7c5;border:0;border-radius:3px 3px 12px 12px;box-shadow:0 14px 25px #a8506720;perspective:600px}.envelope:before{content:"";position:absolute;inset:0;background:#f4c9d3;clip-path:polygon(0 0,50% 55%,100% 0,100% 100%,0 100%);z-index:2}.flap{position:absolute;inset:0;background:#e5a4b6;clip-path:polygon(0 0,100% 0,50% 60%);transform-origin:top;transition:transform .6s;z-index:3}.seal{position:absolute;left:calc(50% - 19px);top:65px;font-size:35px;color:#c85e80;z-index:4}.envelope:hover .flap{transform:rotateX(30deg)}.letter{background:var(--paper);border:1px solid #eed0d7;border-radius:8px;padding:26px;margin:25px auto;max-width:360px;box-shadow:0 12px 40px #b15d7120;animation:appear .6s ease both}.letter h2{font-weight:normal;font-size:28px}.reset{border:0;background:none;color:#a56b7e;text-decoration:underline;text-underline-offset:5px;margin-top:25px;font-size:13px;padding:10px}.footer{position:absolute;bottom:32px;font-size:11px;letter-spacing:2px;color:#be8d99} @keyframes bob{50%{transform:translateY(-7px) rotate(2deg)}}@keyframes beat{50%{transform:scale(1.08)}}@keyframes appear{from{opacity:0;transform:translateY(15px)}to{opacity:1;transform:translateY(0)}}
@media(max-width:480px){.stage{min-height:90svh;padding:65px 20px}.eyebrow{margin-bottom:20px}.mascot{width:125px;height:130px}.btn{padding:14px 24px}}
@media(prefers-reduced-motion:reduce){*,*:before,*:after{animation:none!important;transition:none!important}}
</style>
</head>
<body>
<main class="stage">
<div class="speckles" aria-hidden="true" id="petals"></div>
<div class="panel">
<p class="eyebrow">A little question, just for you</p>
<!-- Original inline illustration: no external images or fonts required. -->
<svg class="mascot" viewBox="0 0 160 165" role="img" aria-label="A little bear holding a pink heart">
<g stroke="#71645e" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round">
<path fill="#fcf8ec" d="M48 42C22 26 24 7 42 14Q55 15 59 32M103 32Q115 7 131 18Q146 33 122 46"/>
<path fill="#fcf8ec" d="M42 81C17 48 43 25 80 27C121 25 146 47 122 82L127 137Q123 153 109 146L99 132L66 132Q57 156 44 144Z"/>
<ellipse fill="#544d47" stroke="none" cx="61" cy="61" rx="3" ry="4"/><ellipse fill="#544d47" stroke="none" cx="101" cy="61" rx="3" ry="4"/>
<path fill="none" d="M73 69Q80 80 87 69"/><ellipse fill="#efb4bb" stroke="none" cx="48" cy="72" rx="9" ry="5"/><ellipse fill="#efb4bb" stroke="none" cx="112" cy="72" rx="9" ry="5"/>
<path class="heart" fill="#e98ca5" stroke="#cb6d89" d="M80 132C13 95 57 74 80 95C103 74 147 95 80 132Z"/>
<path fill="#fcf8ec" d="M42 93Q67 85 65 103Q59 112 43 105M118 93Q93 85 95 103Q101 112 117 105"/>
</g><text x="133" y="63" class="tiny-heart">♡</text><text x="12" y="88" class="tiny-heart">♡</text>
</svg>
<section id="question">
<h1>Do you love me?</h1><p class="sub">Be honest… my heart is listening ♡</p>
<div class="choices"><button class="btn" id="yes">♡ YES</button><button class="btn no" id="no">× NO</button></div>
<p class="hint" id="hint">A tiny question. A very big feeling.</p>
</section>
<section id="measuring" hidden aria-label="Measuring love">
<p class="meter-label" id="meterLabel">♡ Measuring love level… ♡</p><output class="count" id="count">0%</output><div class="track"><div class="fill" id="fill"></div></div><p class="sub">Looks like there's a little more than expected…</p>
</section>
<section id="result" hidden>
<h1>I KNEW IT! ♡</h1><p>I love you <strong>1000%</strong>.</p>
<button class="envelope" id="envelope" aria-label="Open your love letter" aria-expanded="false" aria-controls="letter"><span class="flap"></span><span class="seal">♥</span></button>
<p class="hint" id="openHint">A little love letter. Tap to open.</p>
<article class="letter" id="letter" hidden><h2>To my favorite person,</h2><p>You make the ordinary days feel special. Every little moment with you is my favorite place to be.</p><p>If I could choose anyone,<br>I'd choose you. Every single time.</p><p>All my love, always. ♡</p></article>
<button class="reset" id="reset">Ask me again ♡</button>
</section>
</div>
<span class="footer">MADE WITH A WHOLE LOT OF LOVE</span>
</main>
<script>
// Small interaction layer: runaway button, animated meter, and letter reveal.
const $ = id => document.getElementById(id);
const reducedMotion = matchMedia('(prefers-reduced-motion: reduce)').matches;
for(let i=0;i<22;i++){
 const petal=document.createElement('span');petal.className='petal';petal.textContent=['♡','♥','✿','·'][i%4];
 petal.style.cssText=`--x:${(i*47)%100}%;--time:${12+i%7}s;--delay:${-i*1.7}s;--size:${12+i%5*4}px`;
 $('petals').append(petal);
}
let dodges=0, busy=false;
function dodge(){
 if(busy)return;
 const button=$('no');const r=button.getBoundingClientRect();
 const maxX=Math.max(12,innerWidth-r.width-18),maxY=Math.max(12,innerHeight-r.height-18);
 let x,y;
 // Alternate sides so the new position is away from the pointer.
 x=r.left<innerWidth/2?maxX*.8:18;
 y=Math.min(maxY,Math.max(18,innerHeight*(.22+Math.random()*.5)));
 button.style.position='fixed';button.style.left=x+'px';button.style.top=y+'px';
 // Move out of the animated panel so fixed positioning is viewport-relative.
 document.body.append(button);
 $('hint').textContent=['Oops… that button is a little shy!','Are you sure? 🥺','My heart votes YES ♡'][dodges++%3];
}
$('no').addEventListener('pointerenter',e=>{if(e.pointerType==='mouse'&&!reducedMotion)dodge()});
$('no').addEventListener('click',dodge);
$('yes').addEventListener('click',()=>{
 if(busy)return;busy=true;$('question').hidden=true;$('no').hidden=true;$('measuring').hidden=false;
 const start=performance.now(),duration=reducedMotion?0:4800;
 function tick(now){const progress=duration?Math.min((now-start)/duration,1):1;const value=Math.round(progress*1000);
 $('count').textContent=value+'%';$('fill').style.width=progress*100+'%';
 if(value>=1000)$('meterLabel').textContent='OVERFLOWING WITH LOVE! ♡';
 if(progress<1)requestAnimationFrame(tick);else setTimeout(()=>{$('measuring').hidden=true;$('result').hidden=false;$('envelope').focus({preventScroll:true})},1000);
 }requestAnimationFrame(tick);
});
$('envelope').addEventListener('click',()=>{
 const open=$('letter').hidden;$('letter').hidden=!open;$('envelope').setAttribute('aria-expanded',String(open));
 $('openHint').textContent=open?'Sealed with a kiss ♡':'A little love letter. Tap to open.';
 if(open)$('letter').scrollIntoView({behavior:reducedMotion?'instant':'smooth',block:'nearest'});
});
$('reset').addEventListener('click',()=>{
 busy=false;dodges=0;$('result').hidden=true;$('letter').hidden=true;$('question').hidden=false;$('no').hidden=false;
 $('no').removeAttribute('style');document.querySelector('.choices').append($('no'));
 $('count').textContent='0%';$('fill').style.width='0%';$('meterLabel').textContent='♡ Measuring love level… ♡';
 $('hint').textContent='A tiny question. A very big feeling.';$('openHint').textContent='A little love letter. Tap to open.';
 $('envelope').setAttribute('aria-expanded','false');$('yes').focus({preventScroll:true});
});
addEventListener('resize',()=>{if($('no').style.position){$('no').removeAttribute('style');document.querySelector('.choices').append($('no'))}});
</script>
</body>
</html>
