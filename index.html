<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For Shamatha 💜</title>

<style>
*{box-sizing:border-box}
body{
  margin:0;min-height:100vh;display:flex;align-items:center;
  justify-content:center;padding:20px;overflow:hidden;
  font-family:'Trebuchet MS',sans-serif;color:#58447f;
  background:linear-gradient(-45deg,#f7f0ff,#d9c8ff,#eee5ff,#c6b1ff);
  background-size:400% 400%;animation:bg 12s ease infinite;
}
@keyframes bg{0%,100%{background-position:0% 50%}50%{background-position:100% 50%}}
.card{
  width:100%;max-width:490px;padding:34px 23px;
  position:relative;z-index:1;
  border:2px solid #ffffffb8;border-radius:30px;
  background:#ffffffd9;backdrop-filter:blur(12px);
  box-shadow:0 20px 60px #7154a52b;text-align:center;
  animation:enter 1s ease;
}
@keyframes enter{from{opacity:0;transform:translateY(25px) scale(.96)}to{opacity:1;transform:none}}
h1{font-size:clamp(30px,8vw,43px);margin:12px 0;color:#674a9b}
p{font-size:18px;line-height:1.7}
.small{font-size:13px;letter-spacing:3px;text-transform:uppercase;color:#9478c6}
.envelope{
  font-size:100px;cursor:pointer;display:inline-block;
  animation:bounce 1.8s infinite;filter:drop-shadow(0 8px 8px #a38bce44);
}
@keyframes bounce{0%,100%{transform:translateY(0) rotate(-3deg)}50%{transform:translateY(-12px) rotate(3deg)}}
button{
  border:0;border-radius:30px;padding:14px 21px;
  font-size:16px;font-weight:bold;cursor:pointer;
  transition:transform .2s,box-shadow .2s;font-family:inherit;
}
button:hover{transform:translateY(-3px);box-shadow:0 8px 20px #7e61ac35}
.open-btn{background:#9675e8;color:white}
.buttons{display:flex;gap:12px;justify-content:center;flex-wrap:wrap;margin-top:24px}
.yes{background:linear-gradient(135deg,#a88cf0,#8061d1);color:white}
.no{background:#eee5ff;color:#634c91;border:1px solid #d9caff}
#letter{display:none}
#letter.show{display:block;animation:reveal 1s ease}
@keyframes reveal{from{opacity:0;transform:translateY(35px) scale(.9)}to{opacity:1;transform:none}}
.heart{font-size:42px;animation:heartbeat 1.3s infinite;display:inline-block}
@keyframes heartbeat{50%{transform:scale(1.18)}}
#reply{margin-top:22px;font-weight:bold;font-size:18px;line-height:1.6;min-height:30px}
.float{
  position:fixed;bottom:-40px;pointer-events:none;
  animation:rise linear forwards;z-index:0;
}
@keyframes rise{to{transform:translateY(-115vh) rotate(360deg);opacity:0}}
.footer{font-size:12px;color:#9988b8;margin-top:22px}
#rose-scene{
  position:fixed;inset:0;z-index:5;display:grid;place-items:center;
  background:#060208;cursor:pointer;
}
#rose-scene[hidden]{display:none}
#rose-canvas{width:min(100vw,100svh);height:min(100vw,100svh);display:block}
#rose-hint{
  position:fixed;bottom:14px;left:0;right:0;margin:0;
  color:#ffd1dc;font-size:13px;text-align:center;opacity:.8;
}
#reject-scene{
  position:fixed;inset:0;z-index:6;display:grid;place-items:center;
  padding:24px;background:#060208;color:#ffd1dc;cursor:pointer;text-align:center;
}
#reject-scene[hidden]{display:none}
#reject-copy{
  margin:0;font-size:clamp(32px,8vw,60px);line-height:1.35;
  font-family:Georgia,"Times New Roman",serif;
  text-shadow:0 0 24px #e83c6880;
}
#reject-copy.animate{animation:rejectReveal 1s ease both}
@keyframes rejectReveal{
  from{opacity:0;transform:translateY(18px) scale(.95)}
  to{opacity:1;transform:translateY(0) scale(1)}
}
#reject-hint{
  position:fixed;bottom:14px;left:0;right:0;margin:0;
  color:#ffd1dc;font-size:13px;opacity:.8;
}
</style>
</head>

<body>
<main class="card">

  <section id="intro">
    <div class="small">A secret message for you</div>
    <div class="envelope" onclick="openLetter()">💌</div>
    <h1>Open This!</h1>
    <p>Someone has something special to tell you... 🫣💜</p>
    <button class="open-btn" onclick="openLetter()">Open my letter ✨</button>
  </section>

  <section id="letter">
    <div class="heart">💜</div>
    <h1>Hey, Shamatha! 🪻</h1>

    <p>
      I have a crush on you... 🫠<br>
      <b>Since our school days!</b>
    </p>

    <p style="color:#8a68cf;font-weight:bold">
      Not even the most expensive camera can capture you...
      <br>
      The way my eyes do 📽️🙃👀
    </p>

    <p>Anyway... I have one little question for you. 💌</p>
    <h2>Will you accept my proposal? 🥹</h2>

    <div class="buttons">
      <button class="yes" onclick="accept()">1. Accept 🫠💜</button>
      <button class="no" onclick="reject()">2. Reject 🙂</button>
    </div>

    <div id="reply" aria-live="polite"></div>
    <div class="footer">Whatever your answer, keep smiling! 💜</div>
  </section>
</main>

<div id="rose-scene" role="button" tabindex="0"
     aria-label="Animated rose made from love phrases. Click or press Escape to return to the proposal." hidden>
  <canvas id="rose-canvas" width="800" height="800"></canvas>
  <p id="rose-hint">Click anywhere to return to the proposal</p>
</div>
<div id="reject-scene" role="button" tabindex="0"
     aria-label="Sry for proposing. Click or press Escape to return to the proposal." hidden>
  <p id="reject-copy">Sry for proposing ]:<br>And I think you got angry.</p>
  <p id="reject-hint">Click anywhere or press Escape to return to the proposal</p>
</div>

<script>
const SHEETS_WEB_APP_URL = 'https://script.google.com/macros/s/AKfycbxpd0d4P19NCT2KU2mKiSE-D87G8RmVv0PK10H8bUAhueou21PssrV7keouBt4XzjOR/exec';
const ROSE_WIDTH = 800;
const ROSE_DURATION = 10000;
const ROSE_TICK = 16;
const ROSE_LIFT = 32;
const ROSE_BG = '#060208';
const roseCanvas = document.getElementById('rose-canvas');
const roseContext = roseCanvas.getContext('2d');
const roseBaseCanvas = document.createElement('canvas');
roseBaseCanvas.width = ROSE_WIDTH;
roseBaseCanvas.height = ROSE_WIDTH;
const roseBaseContext = roseBaseCanvas.getContext('2d');
const roseScene = document.getElementById('rose-scene');
const rejectScene = document.getElementById('reject-scene');

const ROSE_PHRASES = [
  'I LOVE YOU', 'I love you', 'Te amo', 'Ti amo', "Je t'aime",
  'Ich liebe dich', 'Eu te amo', 'Seni seviyorum', 'Я тебя люблю',
  '사랑해', '愛してる', '我爱你', 'मैं तुमसे प्यार करती हूँ',
  'मैं तुमसे प्यार करता हूँ', "Σ' αγαπώ", 'Ik hou van jou',
  'Jag älskar dig', 'Kocham cię', 'ฉันรักคุณ', 'Anh yêu em',
  'Aku cinta kamu', 'Mahal kita', 'אני אוהבת אותך', 'أحبك',
  'నేను నిన్ను ప్రేమిస్తున్నాను', 'நான் உன்னை காதலிக்கிறேன்',
  'আমি তোমাকে ভালোবাসি', 'Volim te', 'Te iubesc', 'Ljubim te',
  'Nakupenda', 'Я тебе кохаю', 'Miluji tě', 'Szeretlek',
  'Rakastan sinua', 'Jeg elsker dig'
];
const ROSE_ACCENTS = [
  'LOVE', 'TE AMO', 'AMOUR', 'TI AMO', 'I LOVE YOU', 'AMOR',
  '愛してる', '사랑해', '我爱你', 'LOVE YOU', "JE T'AIME",
  'SZERETLEK', 'NAKUPENDA'
];
const ROSE_SHORT_PHRASES = [
  'Te amo', 'Ti amo', 'AMOR', 'LOVE', '愛してる', '사랑해', '我爱你',
  'Amour', 'I love you', 'Mahal kita', 'Te iubesc', 'Volim te',
  'Szeretlek', 'Miluji tě', 'Nakupenda'
];
const ROSE_HEAD_WORDS = ROSE_PHRASES.concat([
  'LOVE', 'LOVE', 'LOVE YOU', 'AMOR', 'AMOR', 'AMOUR', 'AMOUR',
  'AMORE', 'LIEBE', 'TE AMO', 'TE AMO', 'TI AMO', 'TI AMO',
  'TE QUIERO', 'TE QUIERO', "JE T'AIME", 'I LOVE YOU', 'I LOVE YOU',
  '愛', '愛してる', '愛してる', '사랑', '사랑해', '사랑해', '我爱你',
  'Mahal kita', 'รักคุณ', 'ANH YÊU EM', 'तुमसे प्यार है',
  'నిన్ను ప్రేమిస్తున్నా', 'உன்னை காதலிக்கிறேன்', 'ভালোবাসি',
  'أحبك', 'LOVE', 'AMOR', 'AMOUR', 'Nakupenda', 'Szeretlek'
]);
const ROSE_HEAD_SIZES = [7, 8, 9, 10, 11, 12, 13, 14];
const ROSE_HEAD_WEIGHTS = [2, 4, 5, 5, 4, 2, 1, 0.5];
const ROSE_HEAD_SHAPES = [
  roseEllipse(400, 180, 145, 90),
  roseEllipse(330, 180, 120, 83),
  roseEllipse(470, 180, 120, 83),
  roseEllipse(275, 260, 98, 112),
  roseEllipse(525, 260, 98, 112),
  roseEllipse(338, 325, 118, 126),
  roseEllipse(462, 325, 118, 126),
  [[230, 330], [290, 365], [348, 414], [400, 532],
   [452, 414], [510, 365], [570, 330], [522, 452],
   [400, 542], [278, 452]]
];
const ROSE_STEM = [
  [378, 493], [422, 493], [427, 752], [408, 772], [390, 760], [374, 600]
];
const ROSE_LEFT_LEAF = [
  [395, 594], [359, 554], [304, 535], [244, 541],
  [215, 562], [253, 609], [321, 631], [374, 617]
];
const ROSE_RIGHT_LEAF = [
  [406, 619], [442, 581], [491, 561], [553, 578],
  [578, 600], [535, 640], [476, 660], [425, 649]
];
let roseSeed = 17;
let roseFrame = 0;
let roseAnimationFrame = 0;
let roseItems = [];
let roseActive = [];
let roseStartedAt = 0;

function roseRandom(){
  roseSeed = (roseSeed * 16807) % 2147483647;
  return (roseSeed - 1) / 2147483646;
}

function roseEllipse(cx, cy, rx, ry){
  return Array.from({length:160}, (_, i) => {
    const angle = 2 * Math.PI * i / 160;
    return [cx + rx * Math.cos(angle), cy + ry * Math.sin(angle)];
  });
}

function rosePolygonSpans(poly, y){
  const xs = [];
  for(let i = 0; i < poly.length; i++){
    const [x1, y1] = poly[i];
    const [x2, y2] = poly[(i + 1) % poly.length];
    if((y1 <= y && y < y2) || (y2 <= y && y < y1)){
      xs.push(x1 + (y - y1) * (x2 - x1) / (y2 - y1));
    }
  }
  xs.sort((a, b) => a - b);
  const spans = [];
  for(let i = 0; i + 1 < xs.length; i += 2) spans.push([xs[i], xs[i + 1]]);
  return spans;
}

function roseMergeSpans(spans){
  spans.sort((a, b) => a[0] - b[0]);
  const merged = [];
  for(const [lo, hi] of spans){
    const last = merged[merged.length - 1];
    if(last && lo <= last[1] + 1) last[1] = Math.max(last[1], hi);
    else merged.push([lo, hi]);
  }
  return merged;
}

function roseShapeSpans(polygons, y){
  return roseMergeSpans(polygons.flatMap(poly => rosePolygonSpans(poly, y)));
}

function roseIntersectSpans(aSpans, bSpans, minimum){
  const intersections = [];
  for(const [aLo, aHi] of aSpans){
    for(const [bLo, bHi] of bSpans){
      const lo = Math.max(aLo, bLo);
      const hi = Math.min(aHi, bHi);
      if(hi - lo >= minimum) intersections.push([lo, hi]);
    }
  }
  return roseMergeSpans(intersections);
}

function roseFont(size){
  return `bold ${size}px Georgia, "Times New Roman", Arial, sans-serif`;
}

function roseSize(kind){
  if(kind === 'head'){
    const total = ROSE_HEAD_WEIGHTS.reduce((sum, weight) => sum + weight, 0);
    let value = roseRandom() * total;
    for(let i = 0; i < ROSE_HEAD_SIZES.length; i++){
      value -= ROSE_HEAD_WEIGHTS[i];
      if(value <= 0) return ROSE_HEAD_SIZES[i];
    }
    return ROSE_HEAD_SIZES[0];
  }
  if(kind === 'stem') return [6, 7, 8][Math.floor(roseRandom() * 3)];
  return [7, 8, 9, 10][Math.floor(roseRandom() * 4)];
}

function rosePhrase(kind, size){
  const pool = size >= 14 ? ROSE_ACCENTS :
    kind === 'head' ? ROSE_HEAD_WORDS : ROSE_SHORT_PHRASES;
  return pool[Math.floor(roseRandom() * pool.length)];
}

function roseColor(kind, size, edge){
  let palette;
  if(kind === 'head'){
    palette = size >= 14
      ? ['#c51b49', '#e83c68', '#f16b8b', '#ff91a9', '#ff9ab1', '#ffd0dc']
      : ['#8f0b2b', '#ae1238', '#c41d48', '#d52b53',
         '#b9143d', '#d21e49', '#e33b60', '#f04e73'];
    if(edge) palette.push('#f5a0b3', '#ef6488');
  }else{
    palette = ['#3e8034', '#559c3c', '#72b84b', '#91cf62', '#b1e184'];
    if(size >= 9) palette.push('#a7d486', '#c0e19a');
  }
  return palette[Math.floor(roseRandom() * palette.length)];
}

function roseBuildRegion(polygons, yStart, yEnd, kind){
  const rowHeight = kind === 'head' ? 14 : kind === 'stem' ? 13 : 14;
  const placements = [];
  for(let y = yStart + rowHeight / 2; y < yEnd - rowHeight / 2; y += rowHeight){
    const row = roseIntersectSpans(
      roseShapeSpans(polygons, y - rowHeight / 2 + 1),
      roseShapeSpans(polygons, y + rowHeight / 2 - 1),
      kind === 'head' ? 19 : 16
    );
    for(let [lo, hi] of row){
      lo += kind === 'head' ? 3 : 1;
      hi -= kind === 'head' ? 3 : 1;
      const available = hi - lo;
      if(available < 18) continue;
      const line = [];
      let cursor = lo + roseRandom() * Math.min(3, Math.max(1, available * 0.02));
      while(cursor < hi - 15){
        const remaining = hi - cursor;
        const targetWidth = Math.min(74, Math.max(19, remaining * 0.22));
        const candidates = [];
        const tries = kind === 'head' ? 45 : 55;
        for(let i = 0; i < tries; i++){
          const size = roseSize(kind);
          const text = rosePhrase(kind, size);
          roseContext.font = roseFont(size);
          const width = roseContext.measureText(text).width;
          if(width <= remaining && width >= Math.min(18, remaining * 0.20)){
            candidates.push({
              text, size, width,
              score: Math.abs(width - targetWidth) + roseRandom() * 13
            });
          }
        }
        if(!candidates.length) break;
        candidates.sort((a, b) => a.score - b.score);
        const pick = candidates[Math.floor(roseRandom() * Math.min(4, candidates.length))];
        line.push({x:cursor + pick.width / 2, y, text:pick.text, size:pick.size, width:pick.width, kind});
        cursor += pick.width + (kind === 'head' ? 3 : 1);
      }
      const used = line.reduce((sum, item) => sum + item.width, 0) +
        Math.max(0, line.length - 1) * (kind === 'head' ? 3 : 1);
      const extra = line.length > 1 ? Math.max(0, available - used) / (line.length - 1) : 0;
      line.forEach((item, i) => {
        item.x += extra * i;
        item.edge = i === 0 || i === line.length - 1;
        item.color = roseColor(kind, item.size, item.edge);
        placements.push(item);
      });
    }
  }
  return placements;
}

function rosePrepare(){
  roseSeed = 17;
  roseContext.clearRect(0, 0, ROSE_WIDTH, ROSE_WIDTH);
  roseBaseContext.clearRect(0, 0, ROSE_WIDTH, ROSE_WIDTH);
  const placements = [
    ...roseBuildRegion(ROSE_HEAD_SHAPES, 88, 540, 'head'),
    ...roseBuildRegion([ROSE_LEFT_LEAF], 543, 618, 'leaf'),
    ...roseBuildRegion([ROSE_RIGHT_LEAF], 575, 651, 'leaf'),
    ...roseBuildRegion([ROSE_STEM], 492, 773, 'stem')
  ];
  const outer = placements.filter(item => item.edge)
    .sort((a, b) => Math.atan2(a.y - 300, a.x - 400) - Math.atan2(b.y - 300, b.x - 400));
  const inner = placements.filter(item => !item.edge);
  for(let i = inner.length - 1; i > 0; i--){
    const j = Math.floor(roseRandom() * (i + 1));
    [inner[i], inner[j]] = [inner[j], inner[i]];
  }
  roseItems = outer.concat(inner).map(item => ({
    ...item, dx:(roseRandom() * 12) - 6
  }));
  roseActive = [];
  roseFrame = 0;
}

function roseDraw(item, progress, targetContext = roseContext){
  const context = targetContext;
  const eased = 1 - Math.pow(1 - progress, 3);
  const x = item.x + item.dx * (1 - eased);
  const y = item.y - ROSE_LIFT * (1 - eased);
  const rgb = item.color.match(/[a-f\d]{2}/gi).map(value => parseInt(value, 16));
  context.textAlign = 'center';
  context.textBaseline = 'middle';
  context.font = roseFont(item.size);
  if(progress < 1){
    context.fillStyle = ROSE_BG;
    context.fillText(item.text, x + 1, y + 2);
    context.globalAlpha = eased * eased;
    context.fillStyle = '#6e3947';
    context.fillText(item.text, x, y);
    context.globalAlpha = 1;
    const flash = 0.55 * Math.sin(Math.PI * Math.max(0, Math.min(1, (progress - 0.58) / 0.42)));
    context.fillStyle = `rgb(${rgb.map(channel => Math.round(channel + (255 - channel) * flash)).join(',')})`;
  }else{
    context.fillStyle = item.color;
  }
  context.fillText(item.text, progress < 1 ? x : item.x, progress < 1 ? y : item.y);
}

function roseAnimate(now){
  const elapsed = now - roseStartedAt;
  const interval = ROSE_DURATION / Math.max(1, roseItems.length);
  roseContext.clearRect(0, 0, ROSE_WIDTH, ROSE_WIDTH);
  roseContext.drawImage(roseBaseCanvas, 0, 0);
  while(roseFrame < roseItems.length && roseFrame * interval <= elapsed){
    roseActive.push({item:roseItems[roseFrame], started:roseFrame * interval});
    roseFrame++;
  }
  roseActive = roseActive.filter(active => {
    const progress = Math.min(1, (elapsed - active.started) / 620);
    if(progress >= 1){
      roseDraw(active.item, 1, roseBaseContext);
      return false;
    }
    roseDraw(active.item, progress);
    return true;
  });
  if(roseFrame < roseItems.length || roseActive.length){
    roseAnimationFrame = requestAnimationFrame(roseAnimate);
  }else{
    roseAnimationFrame = 0;
    document.getElementById('rose-hint').textContent =
      'Click anywhere or press Escape to return to the proposal';
  }
}

function showRoseAnimation(){
  if(roseAnimationFrame) cancelAnimationFrame(roseAnimationFrame);
  roseScene.hidden = false;
  document.getElementById('rose-hint').textContent =
    'Click anywhere or press Escape to return to the proposal';
  rosePrepare();
  roseStartedAt = performance.now();
  roseAnimationFrame = requestAnimationFrame(roseAnimate);
}

function closeRoseAnimation(){
  if(roseScene.hidden) return;
  roseScene.hidden = true;
  if(roseAnimationFrame) cancelAnimationFrame(roseAnimationFrame);
  roseAnimationFrame = 0;
}

roseScene.addEventListener('click', closeRoseAnimation);
roseScene.addEventListener('keydown', event => {
  if(event.key === 'Enter' || event.key === ' '){
    event.preventDefault();
    closeRoseAnimation();
  }
});
document.addEventListener('keydown', event => {
  if(event.key === 'Escape') closeRoseAnimation();
});

function showRejectMessage(){
  const message = document.getElementById('reject-copy');
  rejectScene.hidden = false;
  message.classList.remove('animate');
  void message.offsetWidth;
  message.classList.add('animate');
}

function closeRejectMessage(){
  rejectScene.hidden = true;
}

rejectScene.addEventListener('click', closeRejectMessage);
rejectScene.addEventListener('keydown', event => {
  if(event.key === 'Enter' || event.key === ' '){
    event.preventDefault();
    closeRejectMessage();
  }
});
document.addEventListener('keydown', event => {
  if(event.key === 'Escape') closeRejectMessage();
});

function openLetter(){
  document.getElementById('intro').style.display='none';
  document.getElementById('letter').classList.add('show');
  setInterval(makeHeart,500);
}

function accept(){
  recordChoice('Accept');
  document.getElementById('reply').innerHTML =
    'YAYYYY! 💜🥹 You just made my day magical! ✨🪻';
  showRoseAnimation();
}

function reject(){
  recordChoice('Reject');
  document.getElementById('reply').textContent = '';
  celebration();
  showRejectMessage();
}

function recordChoice(choice){
  if (SHEETS_WEB_APP_URL === 'PASTE_YOUR_APPS_SCRIPT_WEB_APP_URL_HERE') return;

  const payload = JSON.stringify({ choice, timestamp: new Date().toISOString() });
  if (navigator.sendBeacon) {
    navigator.sendBeacon(SHEETS_WEB_APP_URL, new Blob([payload], { type: 'text/plain;charset=UTF-8' }));
    return;
  }

  fetch(SHEETS_WEB_APP_URL, {
    method: 'POST',
    mode: 'no-cors',
    headers: { 'Content-Type': 'text/plain;charset=UTF-8' },
    body: payload,
    keepalive: true
  });
}

function makeHeart(){
  const el=document.createElement('div');
  el.className='float';
  el.textContent=['💜','💕','✨','🪻','💗'][Math.floor(Math.random()*5)];
  el.style.left=Math.random()*100+'vw';
  el.style.fontSize=(18+Math.random()*22)+'px';
  el.style.animationDuration=(4+Math.random()*4)+'s';
  document.body.appendChild(el);
  setTimeout(()=>el.remove(),8000);
}

function celebration(){
  for(let i=0;i<35;i++){
    setTimeout(makeHeart,i*70);
  }
}
</script>
</body>
</html>
