<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For Someone Special ♡</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Fredoka:wght@400;500;600;700&family=DM+Sans:wght@400;500;600;700;800&family=Caveat:wght@500;600;700&display=swap');

:root {
  --pink:#ff8eae;
  --pink2:#ffc0d1;
  --red:#f16c86;
  --cream:#fff9f1;
  --ink:#603b4a;
}

* {
  margin:0;
  padding:0;
  box-sizing:border-box;
}

body {
  min-height:100svh;
  overflow-x:hidden;
  font-family:'DM Sans',sans-serif;
  color:var(--ink);
  background:
    radial-gradient(ellipse at 15% 15%,#ffe0e9 0%,transparent 42%),
    radial-gradient(ellipse at 85% 85%,#ffd2d9 0%,transparent 45%),
    linear-gradient(135deg,#fff7f5,#ffe5ec 55%,#fff0f1);
}

button {
  font-family:inherit;
  cursor:pointer;
  -webkit-tap-highlight-color:transparent;
}

.hidden {display:none!important}

#particles {
  position:fixed;
  inset:0;
  overflow:hidden;
  pointer-events:none;
  z-index:0;
}

.particle {
  position:absolute;
  bottom:-50px;
  animation:floatUp linear infinite;
  opacity:.5;
  color:#ef91aa;
}

@keyframes floatUp {
  to {
    transform:translateY(-115vh) rotate(420deg);
    opacity:0;
  }
}

.screen {
  position:relative;
  z-index:2;
  min-height:100svh;
  display:flex;
  align-items:center;
  justify-content:center;
  padding:35px 20px;
}

/* HOME */

.intro-card {
  width:min(100%,520px);
  text-align:center;
  padding:48px 28px 38px;
  border:1px solid rgba(255,255,255,.85);
  border-radius:36px;
  background:rgba(255,255,255,.57);
  backdrop-filter:blur(25px);
  box-shadow:0 25px 65px rgba(204,111,137,.13),
  inset 0 2px 4px white;
  animation:cardEnter .8s ease;
}

@keyframes cardEnter {
  from {opacity:0;transform:translateY(30px) scale(.94)}
  to {opacity:1;transform:translateY(0) scale(1)}
}

.top-label {
  display:inline-flex;
  gap:8px;
  padding:9px 15px;
  border-radius:30px;
  border:1px solid #fff;
  background:rgba(255,255,255,.7);
  color:#cb718d;
  font-size:10px;
  font-weight:800;
  letter-spacing:2px;
  margin-bottom:27px;
}

.hero-heart {
  width:112px;
  height:112px;
  margin:0 auto 23px;
  display:grid;
  place-items:center;
  border-radius:34px;
  transform:rotate(-7deg);
  background:linear-gradient(145deg,#ffd8e3,#ff9eb8);
  border:2px solid white;
  box-shadow:8px 9px 0 rgba(208,111,139,.15),inset 0 3px 8px white;
  animation:heartFloat 3s ease-in-out infinite;
}

.hero-heart svg {width:65px}

@keyframes heartFloat {
  0%,100% {transform:translateY(0) rotate(-7deg)}
  50% {transform:translateY(-9px) rotate(5deg)}
}

h1 {
  font-family:'Fredoka',sans-serif;
  font-size:clamp(29px,7vw,43px);
  line-height:1.16;
  color:#a94d6d;
  text-shadow:2px 3px 0 rgba(240,146,172,.25);
}

h1 span {color:#ef7798}

.description {
  max-width:340px;
  margin:16px auto 29px;
  color:#a77c89;
  font-size:13px;
  line-height:1.8;
}

.button-area {
  min-height:75px;
  position:relative;
  display:flex;
  align-items:center;
  justify-content:center;
  gap:13px;
  flex-wrap:wrap;
}

.clay-btn {
  border:1px solid white;
  padding:14px 29px;
  min-width:116px;
  border-radius:18px;
  font-size:15px;
  font-weight:800;
  transition:all .3s cubic-bezier(.2,1.5,.4,1);
}

.yes-btn {
  color:white;
  background:linear-gradient(145deg,#ff9db8,#eb668d);
  box-shadow:0 6px 0 #cf6282,0 11px 22px rgba(221,103,139,.22),inset 0 3px 5px rgba(255,255,255,.6);
}

.yes-btn:hover {transform:translateY(-4px) scale(1.06)}

.yes-btn:active {
  transform:translateY(4px) scale(.96);
  box-shadow:0 2px 0 #cf6282;
}

.no-btn {
  color:#aa7787;
  background:linear-gradient(145deg,#fff,#ffeaf0);
  box-shadow:0 5px 0 #e9c6d0,inset 0 2px 4px white;
  position:relative;
}

.counter {
  margin-top:22px;
  color:#c48a9b;
  font-size:11px;
  letter-spacing:1px;
}

/* CELEBRATION */

#celebration {
  position:fixed;
  inset:0;
  z-index:10;
  background:linear-gradient(145deg,#fff3f5,#ffdae5,#fff1ef);
  display:flex;
  align-items:center;
  justify-content:center;
  overflow:hidden;
}

.celebrate-content {
  text-align:center;
  position:relative;
  z-index:3;
}

.big-heart {
  width:130px;
  height:130px;
  margin:auto;
  display:grid;
  place-items:center;
  animation:heartSpin 1.6s ease-in-out forwards;
}

.big-heart svg {
  width:110px;
  filter:drop-shadow(0 15px 15px rgba(212,93,128,.23));
}

@keyframes heartSpin {
  0% {transform:scale(.1) rotate(-360deg)}
  65% {transform:scale(1.3) rotate(20deg)}
  100% {transform:scale(1) rotate(0)}
}

.big-heart.boom {animation:boom .65s ease-in forwards}

@keyframes boom {
  0% {transform:scale(1);opacity:1}
  55% {transform:scale(1.7);opacity:.8}
  100% {transform:scale(2.8);opacity:0}
}

.celebrate-title {
  font-family:'Fredoka',sans-serif;
  color:#c6557b;
  font-size:clamp(35px,8vw,55px);
  margin-top:15px;
  animation:fadeUp .8s .5s both;
}

.celebrate-sub {
  color:#ac8190;
  margin-top:10px;
  font-size:13px;
  animation:fadeUp .8s .7s both;
}

@keyframes fadeUp {
  from {opacity:0;transform:translateY(20px)}
  to {opacity:1;transform:translateY(0)}
}

.burst {
  position:absolute;
  pointer-events:none;
  font-size:24px;
  animation:burstFly 2.5s ease-out forwards;
}

@keyframes burstFly {
  from {transform:translate(0,0) scale(.3) rotate(0);opacity:1}
  to {transform:translate(var(--x),var(--y)) scale(1.5) rotate(360deg);opacity:0}
}

/* ENVELOPE */

#envelopeScreen {text-align:center;flex-direction:column}

.envelope-caption {
  font-family:'Fredoka',sans-serif;
  color:#b85c7b;
  font-size:28px;
  margin-bottom:38px;
}

.envelope {
  width:220px;
  height:155px;
  position:relative;
  cursor:pointer;
  perspective:800px;
  animation:envelopeFloat 3s ease-in-out infinite;
  filter:drop-shadow(0 15px 17px rgba(188,93,124,.15));
}

@keyframes envelopeFloat {
  0%,100% {transform:translateY(0) rotate(-2deg)}
  50% {transform:translateY(-13px) rotate(2deg)}
}

.env-body {
  position:absolute;
  inset:0;
  background:#f59ab4;
  border:2px solid white;
  border-radius:9px;
  overflow:hidden;
}

.env-left,.env-right,.env-bottom {position:absolute;inset:0}

.env-left {
  background:#ed83a2;
  clip-path:polygon(0 0,50% 55%,0 100%);
}

.env-right {
  background:#e77d9d;
  clip-path:polygon(100% 0,50% 55%,100% 100%);
}

.env-bottom {
  background:#f7abc0;
  clip-path:polygon(0 100%,50% 45%,100% 100%);
}

.env-flap {
  position:absolute;
  inset:0;
  background:#ffbfd0;
  clip-path:polygon(0 0,100% 0,50% 65%);
  transform-origin:top;
  transition:transform .8s;
  z-index:4;
}

.seal {
  position:absolute;
  width:44px;
  height:44px;
  left:50%;
  top:57%;
  transform:translate(-50%,-50%);
  z-index:5;
  background:#fff0f3;
  border:2px solid white;
  border-radius:50%;
  display:grid;
  place-items:center;
  color:#e66d91;
  font-size:23px;
  box-shadow:0 3px 8px #d87c96;
  transition:.4s;
}

.envelope.opened .env-flap {transform:rotateX(180deg)}
.envelope.opened .seal {opacity:0;transform:translate(-50%,-50%) scale(.2)}
.envelope.opened {animation:none}

.env-hint {
  margin-top:34px;
  color:#bb8295;
  font-size:12px;
  letter-spacing:1px;
}

/* BOOK */

#letterScreen {
  padding:35px 16px;
  flex-direction:column;
}

.book-heading {
  text-align:center;
  margin-bottom:22px;
}

.book-heading h2 {
  font-family:'Fredoka',sans-serif;
  font-size:27px;
  color:#bb6380;
}

.book-heading p {
  color:#bd8a99;
  font-size:11px;
  margin-top:6px;
  letter-spacing:1px;
}

.book-scene {
  width:min(100%,480px);
  height:530px;
  position:relative;
  perspective:1800px;
  filter:drop-shadow(0 20px 25px rgba(176,99,124,.16));
}

.book {
  width:100%;
  height:100%;
  position:relative;
  transform-style:preserve-3d;
}

.book-base {
  position:absolute;
  inset:0;
  background:#fff9ef;
  border-radius:5px 18px 18px 5px;
  box-shadow:inset 8px 0 0 #e9b7c4,inset -3px 0 0 #e9d5d0;
  overflow:hidden;
}

.book-base::after {
  content:"";
  position:absolute;
  top:0;
  bottom:0;
  left:50%;
  width:2px;
  background:rgba(191,142,145,.25);
}

.paper-stack {
  position:absolute;
  right:0;
  top:4px;
  width:7px;
  height:calc(100% - 8px);
  background:repeating-linear-gradient(to bottom,#e8d8d0 0 2px,#fff8ee 2px 4px);
  border-radius:0 8px 8px 0;
}

.book-page {
  position:absolute;
  inset:0;
  padding:34px 27px;
  background:
    repeating-linear-gradient(to bottom,transparent 0,transparent 31px,rgba(222,180,185,.24) 32px),
    #fffaf2;
  border-radius:4px 15px 15px 4px;
  border:1px solid #f1dfd9;
  transform-origin:left center;
  transform-style:preserve-3d;
  backface-visibility:hidden;
  -webkit-backface-visibility:hidden;
  overflow:hidden;
  transition:transform 1s cubic-bezier(.65,0,.25,1);
  box-shadow:inset 5px 0 9px rgba(197,142,150,.09);
}

.book-page::after {
  content:"";
  position:absolute;
  inset:0;
  pointer-events:none;
  background:linear-gradient(90deg,rgba(181,117,131,.1),transparent 12%,transparent 92%,rgba(194,143,145,.08));
}

.book-page.flipped {
  transform:rotateY(-180deg);
}

.page-content {
  position:relative;
  z-index:1;
  height:100%;
  display:flex;
  flex-direction:column;
}

.page-top {
  text-align:center;
  color:#d48ba0;
  font-size:9px;
  font-weight:800;
  letter-spacing:2px;
  margin-bottom:16px;
}

.page-title {
  font-family:'Caveat',cursive;
  text-align:center;
  color:#c65c7b;
  font-size:39px;
  margin-bottom:19px;
}

.page-text {
  font-size:13px;
  line-height:2;
  color:#85616d;
  font-weight:500;
}

.page-text strong {color:#d16d89}

.page-signature {
  margin-top:auto;
  text-align:right;
  font-family:'Caveat',cursive;
  font-size:23px;
  color:#bd718b;
  padding-top:15px;
}

.page-flower {
  text-align:center;
  font-size:21px;
  margin-top:13px;
}

.page-number {
  text-align:center;
  color:#ce9ba7;
  font-size:10px;
  letter-spacing:2px;
  margin-top:10px;
}

.poem {
  font-family:'Caveat',cursive;
  font-size:23px;
  line-height:1.65;
  text-align:center;
  color:#a75c78;
  padding:5px 0;
}

.poem-separator {
  width:48px;
  height:2px;
  border-radius:5px;
  background:#f0b3c4;
  margin:16px auto;
}

.page-3-title {
  font-family:'Caveat',cursive;
  text-align:center;
  font-size:38px;
  color:#c65c7b;
  margin:35px 0 20px;
}

.page-3-heart {
  font-size:58px;
  text-align:center;
  margin:25px 0;
  animation:heartFloat 3s infinite;
}

.page-3-message {
  text-align:center;
  font-size:13px;
  line-height:2;
  color:#956d7b;
}

/* Page layers */
#page1 {z-index:3}
#page2 {z-index:2}
#page3 {z-index:1}

.book-controls {
  display:flex;
  align-items:center;
  justify-content:center;
  gap:18px;
  margin-top:22px;
}

.page-btn {
  min-width:105px;
  border:1px solid white;
  border-radius:15px;
  padding:12px 17px;
  font-size:12px;
  font-weight:800;
  color:#a45c76;
  background:linear-gradient(145deg,#fff,#ffe8ef);
  box-shadow:0 4px 0 #e8c5d0;
  transition:.2s;
}

.page-btn:active {
  transform:translateY(3px);
  box-shadow:0 1px 0 #e8c5d0;
}

.page-btn.primary {
  color:white;
  background:linear-gradient(145deg,#ff9db8,#e97898);
  box-shadow:0 4px 0 #cf718d;
}

.page-btn:disabled {
  opacity:.35;
  cursor:not-allowed;
}

.page-indicator {
  font-size:12px;
  font-weight:800;
  color:#bd8296;
  min-width:35px;
  text-align:center;
}

.book-hint {
  margin-top:15px;
  text-align:center;
  color:#c28c9d;
  font-size:10px;
  letter-spacing:1px;
}

@media(max-width:400px) {
  .intro-card {padding:36px 20px}
  .clay-btn {padding:13px 24px}
  .book-scene {height:510px}
  .book-page {padding:29px 21px}
  .page-text {font-size:12px;line-height:1.95}
  .poem {font-size:21px}
  .page-title {font-size:35px}
}

@media(max-height:750px) {
  .book-scene {height:480px}
  .book-page {padding-top:25px;padding-bottom:23px}
  .page-title {margin-bottom:12px}
  .page-text {line-height:1.8}
}
</style>
</head>

<body>

<div id="particles"></div>

<!-- HOME -->
<main class="screen" id="homeScreen">
  <section class="intro-card">

    <div class="top-label">♡ A LITTLE QUESTION FOR YOU</div>

    <div class="hero-heart">
      <svg viewBox="0 0 100 100" fill="none">
        <path d="M50 85S8 60 8 33C8 12 35 4 50 29C65 4 92 12 92 33C92 60 50 85 50 85Z"
        fill="#ef668b" stroke="#fff" stroke-width="5" stroke-linejoin="round"/>
        <path d="M26 30Q30 20 40 25" stroke="#fff" stroke-width="5" stroke-linecap="round"/>
      </svg>
    </div>

    <h1 id="question">
      KAMU MAUU GA<br>
      JADII <span>PACARR AKUU?</span>
    </h1>

    <p class="description">
      Ada satu pertanyaan kecil yang sudah lama ingin aku tanyakan.
      Jadi, jawab dengan jujur yaa ♡
    </p>

    <div class="button-area">
      <button class="clay-btn yes-btn" id="yesBtn">IYAAA ♡</button>
      <button class="clay-btn no-btn" id="noBtn">TIDAK</button>
    </div>

    <div class="counter" id="counter">
      MADE WITH ♡ JUST FOR YOU
    </div>

  </section>
</main>

<!-- CELEBRATION -->
<section id="celebration" class="hidden">
  <div class="celebrate-content">
    <div class="big-heart" id="bigHeart">
      <svg viewBox="0 0 100 100" fill="none">
        <path d="M50 88S5 60 5 32C5 8 35 3 50 29C65 3 95 8 95 32C95 60 50 88 50 88Z"
        fill="#f16f91" stroke="white" stroke-width="5"/>
        <path d="M25 27Q31 17 40 23" stroke="white" stroke-width="5" stroke-linecap="round"/>
      </svg>
    </div>
    <h2 class="celebrate-title">YEAYYYYY!! ♡</h2>
    <p class="celebrate-sub">KAMU MEMBUAT HARI INI JADI SPESIAL</p>
  </div>
</section>

<!-- ENVELOPE -->
<section class="screen hidden" id="envelopeScreen">
  <h2 class="envelope-caption">A little letter for you ♡</h2>

  <div class="envelope" id="envelope">
    <div class="env-body">
      <div class="env-left"></div>
      <div class="env-right"></div>
      <div class="env-bottom"></div>
    </div>
    <div class="env-flap"></div>
    <div class="seal">♡</div>
  </div>

  <p class="env-hint">TAP THE ENVELOPE TO OPEN YOUR LETTER</p>
</section>

<!-- THREE PAGE BOOK -->
<section class="screen hidden" id="letterScreen">

  <div class="book-heading">
    <h2>Our Little Love Book ♡</h2>
    <p>THREE PAGES • ONE SPECIAL STORY</p>
  </div>

  <div class="book-scene">
    <div class="book">

      <div class="book-base"></div>
      <div class="paper-stack"></div>

      <!-- PAGE 3 -->
      <article class="book-page" id="page3">
        <div class="page-content">

          <div class="page-top">A NEW CHAPTER BEGINS • 03</div>

          <h2 class="page-3-title">Untuk Kita ♡</h2>

          <div class="page-3-heart">💗</div>

          <p class="page-3-message">
            Hari ini menjadi salah satu cerita
            yang ingin selalu aku ingat.
            <br><br>
            Semoga kita terus tumbuh bersama,
            saling mengerti, saling menghargai,
            dan tidak berhenti menciptakan
            kenangan indah.
            <br><br>
            <strong>YOU ARE MY FAVORITE STORY.</strong>
          </p>

          <div class="page-signature">Forever with love ♡</div>
          <div class="page-flower">🌷 🌸 💗 🌸 🌷</div>
          <div class="page-number">— 03 —</div>

        </div>
      </article>

      <!-- PAGE 2 -->
      <article class="book-page" id="page2">
        <div class="page-content">

          <div class="page-top">A LITTLE POEM FOR YOU • 02</div>

          <h2 class="page-title">Pantun Untukmu</h2>

          <div class="poem">
            Pergi ke taman memetik melati,<br>
            Melihat kupu terbang menari.<br>
            Sejak kamu hadir di hati,<br>
            Hari-hariku terasa berseri.
          </div>

          <div class="poem-separator"></div>

          <div class="poem">
            Bunga mawar tumbuh di taman,<br>
            Harumnya sampai ke tepi jalan.<br>
            Bukan sekadar ingin berpacaran,<br>
            Aku ingin kita saling bertahan.
          </div>

          <div class="poem-separator"></div>

          <div class="poem">
            Langit senja berwarna jingga,<br>
            Bintang bersinar menemani malam.<br>
            Semoga kita selalu bersama,<br>
            Menjaga cinta hingga mendalam.
          </div>

          <div class="page-signature">Dari aku, untuk kamu ♡</div>
          <div class="page-number">— 02 —</div>

        </div>
      </article>

      <!-- PAGE 1 -->
      <article class="book-page" id="page1">
        <div class="page-content">

          <div class="page-top">A SPECIAL LETTER • JUST FOR YOU</div>

          <h2 class="page-title">Untuk Kamu ♡</h2>

          <div class="page-text">
            YEAYYY KAMU AKHIRNYAA MAU JADI PACAR AKUU!
            SEKARANG KITA RESMII PACARANN YAAA SAYANGGGGGG. ♡
            <br><br>
            Semoga hubungan ini <strong>LANGGENG TERUS</strong>,
            saling menjaga, saling memahami, saling mendukung,
            dan bertahan lama hingga tua nanti.
            <br><br>
            Aku berharap kita bisa melewati banyak cerita bersama,
            menikmati hari-hari sederhana, dan selalu menghargai
            satu sama lain.
            <br><br>
            MAKASIHH SAYANGGGG SUDAH MENJADI BAGIAN DARI CERITAKU.
            <br><br>
            Semoga ini menjadi awal dari banyak kenangan indah kita. ♡
          </div>

          <div class="page-signature">With lots of love ♡</div>
          <div class="page-flower">🌷 🌸 💗 🌷</div>
          <div class="page-number">— 01 —</div>

        </div>
      </article>

    </div>
  </div>

  <div class="book-controls">
    <button class="page-btn" id="prevBtn" disabled>← KEMBALI</button>
    <span class="page-indicator" id="pageIndicator">1 / 3</span>
    <button class="page-btn primary" id="nextBtn">SELANJUTNYA →</button>
  </div>

  <p class="book-hint" id="bookHint">
    BUKA HALAMAN BERIKUTNYA UNTUK MELANJUTKAN CERITA ♡
  </p>

</section>

<script>
const $ = id => document.getElementById(id);

const home = $('homeScreen');
const celebration = $('celebration');
const envelopeScreen = $('envelopeScreen');
const letterScreen = $('letterScreen');

const yesBtn = $('yesBtn');
const noBtn = $('noBtn');
const question = $('question');
const counter = $('counter');
const envelope = $('envelope');

let noCount = 0;
let noScale = 1;
let envelopeOpened = false;

/* FLOATING BACKGROUND */

const particleContainer = $('particles');
const symbols = ['♡','♥','✿','🌸','✧','❀'];

function createBackgroundParticle() {
  const p = document.createElement('span');
  p.className = 'particle';
  p.textContent = symbols[Math.floor(Math.random()*symbols.length)];

  p.style.left = Math.random()*100+'%';
  p.style.fontSize = (12+Math.random()*20)+'px';
  p.style.animationDuration = (8+Math.random()*12)+'s';
  p.style.animationDelay = Math.random()*3+'s';

  particleContainer.appendChild(p);
  setTimeout(() => p.remove(),22000);
}

setInterval(createBackgroundParticle,500);

for(let i=0;i<15;i++) {
  setTimeout(createBackgroundParticle,i*200);
}

/* NO BUTTON */

function dodgeButton() {
  noCount++;
  noScale = Math.max(.48,noScale-.12);

  noBtn.style.transform = `scale(${noScale})`;

  if(noCount < 4) {
    const x = (Math.random()-.5)*180;
    const y = (Math.random()-.5)*100;

    noBtn.style.position = 'relative';
    noBtn.style.left = x+'px';
    noBtn.style.top = y+'px';

    counter.textContent = `KAMU YAKIN BANGETT... ${noCount}/4 ♡`;
  } else {
    question.innerHTML = 'HARUSSS <span>MAUU!!!!</span>';
    counter.textContent = 'HEHEHE, MASIH ADA PILIHAN KOK ♡';

    noBtn.style.left = '0px';
    noBtn.style.top = '0px';
    noBtn.style.transform = 'scale(.75)';
  }
}

noBtn.addEventListener('click',dodgeButton);

/* LOVE EXPLOSION */

function createBurst() {
  const icons = ['💗','💕','🌸','🌷','💖','✿','♥','✨'];

  for(let i=0;i<45;i++) {
    const el = document.createElement('div');
    el.className = 'burst';
    el.textContent = icons[Math.floor(Math.random()*icons.length)];

    const angle = Math.random()*Math.PI*2;
    const distance = 100+Math.random()*260;

    el.style.left = '50%';
    el.style.top = '50%';

    el.style.setProperty('--x',Math.cos(angle)*distance+'px');
    el.style.setProperty('--y',Math.sin(angle)*distance+'px');

    celebration.appendChild(el);
    setTimeout(()=>el.remove(),2600);
  }
}

yesBtn.addEventListener('click',() => {
  home.classList.add('hidden');
  celebration.classList.remove('hidden');

  createBurst();
  $('bigHeart').classList.add('boom');

  setTimeout(() => {
    celebration.classList.add('hidden');
    envelopeScreen.classList.remove('hidden');
  },2400);
});

/* ENVELOPE */

envelope.addEventListener('click',() => {
  if(envelopeOpened) return;

  envelopeOpened = true;
  envelope.classList.add('opened');

  setTimeout(() => {
    envelopeScreen.classList.add('hidden');
    letterScreen.classList.remove('hidden');
  },1000);
});

/* BOOK PAGE TURN */

const pages = [
  $('page1'),
  $('page2'),
  $('page3')
];

let currentPage = 0;
let isTurning = false;

const prevBtn = $('prevBtn');
const nextBtn = $('nextBtn');
const indicator = $('pageIndicator');
const bookHint = $('bookHint');

function updateBook() {
  indicator.textContent = `${currentPage+1} / 3`;

  prevBtn.disabled = currentPage === 0;
  nextBtn.disabled = currentPage === 2;

  nextBtn.textContent = currentPage === 2
    ? 'SELESAI ♡'
    : 'SELANJUTNYA →';

  if(currentPage === 0) {
    bookHint.textContent = 'BUKA HALAMAN BERIKUTNYA UNTUK MELANJUTKAN CERITA ♡';
  } else if(currentPage === 1) {
    bookHint.textContent = 'MASIH ADA SATU HALAMAN LAGI UNTUK KAMU ♡';
  } else {
    bookHint.textContent = 'TERIMA KASIH SUDAH MEMBACA SURAT KECIL INI ♡';
  }
}

function turnNext() {
  if(isTurning || currentPage >= 2) return;

  isTurning = true;

  const page = pages[currentPage];

  page.style.zIndex = 10;
  page.classList.add('flipped');

  currentPage++;
  updateBook();

  setTimeout(() => {
    page.style.zIndex = currentPage === 1 ? 1 : 0;
    isTurning = false;
  },1050);

  createLetterFlowers();
}

function turnPrevious() {
  if(isTurning || currentPage <= 0) return;

  isTurning = true;

  currentPage--;

  const page = pages[currentPage];

  page.style.zIndex = 10;
  page.classList.remove('flipped');

  updateBook();

  setTimeout(() => {
    page.style.zIndex = 3-currentPage;
    isTurning = false;
  },1050);

  createLetterFlowers();
}

nextBtn.addEventListener('click',() => {
  if(currentPage < 2) {
    turnNext();
  }
});

prevBtn.addEventListener('click',turnPrevious);

updateBook();

/* FLOWER ANIMATION */

function createLetterFlowers() {
  const flowers = ['🌸','💗','🌷','♡','✿'];

  for(let i=0;i<9;i++) {
    const el = document.createElement('span');

    el.textContent = flowers[Math.floor(Math.random()*flowers.length)];

    Object.assign(el.style,{
      position:'fixed',
      left:Math.random()*100+'%',
      top:'100%',
      fontSize:(18+Math.random()*15)+'px',
      pointerEvents:'none',
      zIndex:20,
      transition:'transform 2s ease, opacity 2s ease'
    });

    document.body.appendChild(el);

    requestAnimationFrame(()=>{
      el.style.transform=`translateY(-${110+Math.random()*400}px) rotate(360deg)`;
      el.style.opacity='0';
    });

    setTimeout(()=>el.remove(),2200);
  }
}
</script>

</body>
</html>
