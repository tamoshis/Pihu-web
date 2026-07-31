<!DOCTYPE html>  <html lang="en">  
<head>  
<meta charset="UTF-8">  
<meta name="viewport" content="width=device-width, initial-scale=1.0">  
<title>For My Beautiful Pihu ❤️</title>  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&family=Parisienne&display=swap" rel="stylesheet">  <style>  
* {  
  margin: 0;  
  padding: 0;  
  box-sizing: border-box;  
}  
  
body {  
  font-family: 'Poppins', sans-serif;  
  height: 100vh;  
  overflow: hidden;  
  display: flex;  
  justify-content: center;  
  align-items: center;  
  background: linear-gradient(135deg, #180018, #460030, #7a0048);  
  color: white;  
}  
  
/* Background Floating Circles */  
.background {  
  position: fixed;  
  top: 0;  
  left: 0;  
  width: 100%;  
  height: 100%;  
  overflow: hidden;  
  z-index: -2;  
}  
  
.circle {  
  position: absolute;  
  border-radius: 50%;  
  background: rgba(255, 255, 255, .08);  
  animation: float 12s linear infinite;  
}  
  
@keyframes float {  
  0% { transform: translateY(100vh) scale(.2); opacity: 0; }  
  30% { opacity: .7; }  
  100% { transform: translateY(-20vh) scale(1); opacity: 0; }  
}  
  
/* Glassmorphism Card Container */  
.container {  
  width: 90%;  
  max-width: 650px;  
  padding: 40px;  
  border-radius: 30px;  
  background: rgba(255, 255, 255, .08);  
  backdrop-filter: blur(18px);  
  border: 1px solid rgba(255, 255, 255, .12);  
  text-align: center;  
  box-shadow: 0 10px 40px rgba(0, 0, 0, .45);  
  animation: fade 0.8s ease-out;  
  max-height: 90vh;  
  overflow-y: auto;  
}  
  
@keyframes fade {  
  from { opacity: 0; transform: translateY(20px); }  
  to { opacity: 1; transform: translateY(0); }  
}  
  
h1 {  
  font-family: 'Parisienne', cursive;  
  font-size: 50px;  
  color: #ffb6d0;  
  margin-bottom: 20px;  
  text-shadow: 0 0 18px #ff4f93;  
}  
  
p {  
  font-size: 17px;  
  line-height: 1.8;  
  color: #f5f5f5;  
  margin-bottom: 25px;  
}  
  
.btn {  
  padding: 15px 45px;  
  border: none;  
  border-radius: 50px;  
  font-size: 18px;  
  cursor: pointer;  
  font-weight: bold;  
  background: linear-gradient(45deg, #ff4f93, #ff709f);  
  color: white;  
  transition: .4s;  
}  
  
.btn:hover {  
  transform: scale(1.08);  
  box-shadow: 0 0 25px #ff5d9e;  
}  
  
input {  
  padding: 15px;  
  width: 80%;  
  border: none;  
  border-radius: 15px;  
  font-size: 18px;  
  text-align: center;  
  outline: none;  
  margin-bottom: 15px;  
}  
  
/* Audio Control Floating Button */  
.audio-control {  
  position: fixed;  
  top: 20px;  
  right: 20px;  
  z-index: 1000;  
  background: rgba(255, 255, 255, 0.15);  
  backdrop-filter: blur(10px);  
  border: 1px solid rgba(255, 255, 255, 0.3);  
  color: white;  
  border-radius: 50px;  
  padding: 10px 20px;  
  cursor: pointer;  
  font-size: 14px;  
}  
  
/* Interactive Envelope Animation */  
.envelope-wrapper {  
  cursor: pointer;  
  margin: 30px auto;  
  display: inline-block;  
  transition: transform 0.3s;  
}  
  
.envelope-wrapper:hover {  
  transform: scale(1.05);  
}  
  
.envelope {  
  font-size: 80px;  
  animation: pulse 2s infinite;  
}  
  
@keyframes pulse {  
  0% { transform: scale(1); }  
  50% { transform: scale(1.1); }  
  100% { transform: scale(1); }  
}  
  
/* Letter Section Styling with Proper Padding & Margins */  
#letterContent {  
  text-align: left;  
  font-size: 16px;  
  line-height: 1.9;  
  min-height: 220px;  
  white-space: pre-wrap;  
  padding: 20px 25px;  
  margin: 15px 0;  
  background: rgba(0, 0, 0, 0.2);  
  border-radius: 20px;  
  border: 1px solid rgba(255, 255, 255, 0.08);  
}  
  
.math-formula {  
  background: rgba(0, 0, 0, 0.25);  
  padding: 15px;  
  border-radius: 15px;  
  font-family: 'Courier New', Courier, monospace;  
  font-size: 22px;  
  color: #ffb6d0;  
  margin: 20px 0;  
  letter-spacing: 1px;  
}  
</style>  </head>  <body>  <!-- Soft Lofi Background Music -->  <audio id="bgMusic" loop>  
  <source src="https://cdn.pixabay.com/download/audio/2022/05/27/audio_1808fbf07a.mp3?filename=lofi-study-112191.mp3" type="audio/mpeg">  
</audio>  
<button class="audio-control" onclick="toggleAudio()" id="musicBtn">🎵 Play Music</button>  <div class="background" id="background"></div>  <!-- STEP 1: Landing -->  <div class="container" id="step1">  
  <h1>For My Beautiful Bestie ❤️</h1>  
  <p>  
    Hey Pihu. 🌸<br><br>  
    Some people make life a little brighter just by being in it, and you're one of them.<br>  
    So today, I wanted to create something a little different—something made just for you.<br>  
    It's a small collection of thoughts, smiles, and little surprises, all wrapped into one journey.<br>  
    I hope it brings a smile to your face, just like you've brought so many to mine.<br><br>  
    Whenever you're ready... let's begin. ❤️✨  
  </p>  
  <button class="btn" onclick="startJourney()">Begin Journey ✨</button>  
</div>  <!-- STEP 2: Envelope & Letter -->  <div class="container" id="step2" style="display:none;">  
  <h1>💌 A Letter to You</h1>    <div id="envelopeSection" class="envelope-wrapper" onclick="openLetter()">  
    <div class="envelope">✉️</div>  
    <p style="font-size: 15px; color: #ffb6d0;">Tap envelope to open 🌸</p>  
  </div>    <div id="letterContent" style="display:none;"></div>    <br>  
  <button class="btn" id="nextBtn" style="display:none;" onclick="giftPage()">Continue ❤️</button>  
</div>  <!-- STEP 3: Teddy & Bouquet Giphy -->  <div class="container" id="step3" style="display:none;">  
  <h1>A Little Surprise 🎁</h1>    <div style="margin: 20px 0;">  
    <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExM3ZmdXRscTNvZmlzZms4OTkyYmdodndidDFjODQwcDF5ZmtmbmQxbSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/3o7TKoWXm3okO1kgHC/giphy.gif" alt="Teddy Bear holding bouquet" style="width: 220px; border-radius: 20px; box-shadow: 0 10px 20px rgba(0,0,0,0.3);">  
  </div>    <p style="font-size: 20px; font-weight: 600; color: #ffb6d0;">  
    Flowers 💐 for my beautiful Katgolap 🌸  
  </p>  <button class="btn" onclick="puzzlePage()">Next ❤️</button>

</div>  <!-- STEP 4: Quiz Page -->  <div class="container" id="step4" style="display:none;">  
  <h1>One Question For You ❤️</h1>    <p style="font-size: 20px; font-weight: 600; margin-top: 20px;">  
    Who do I love more than you?  
  </p>    <input id="answer" placeholder="Type your answer...">  
  <br>  
  <button class="btn" onclick="checkAnswer()">Submit ❤️</button>    <p id="result" style="margin-top:20px; font-size:18px; min-height: 50px;"></p>  
</div>  <!-- STEP 5: Mathematical Heart Equation Canvas with Axes -->  <div class="container" id="step5" style="display:none;">  
  <h1>Loading Your Surprise ❤️</h1>  
  <p>Plotting our special equation...</p>    <div class="math-formula">  
    (x² + y² - 1)³ = x²y³  
  </div>  <canvas id="heartCanvas" width="350" height="350" style="max-width:100%; background:rgba(0,0,0,.25); border-radius:20px; margin-bottom: 15px;"></canvas>
<br>
<button class="btn" id="drawBtn" onclick="drawHeart()">Draw Equation ❤️</button>

</div>  <!-- STEP 6: Final Slide -->  <div class="container" id="step6" style="display:none;">  
  <h1>Happy Girlfriend's Day ❤️</h1>  
  <div style="font-size:80px; margin-bottom:15px;">❤️</div>  
  <p style="font-size:18px;">  
    Thank you for being part of my life.<br>  
    Thank you for every smile, every laugh, and every beautiful memory.<br><br>  
    I know this is just a little website...<br>  
    But every single page was made with care.<br><br>  
    I hope today reminds you how truly special you are.  
  </p>  
  <button class="btn" onclick="location.reload()">Replay Journey ✨</button>  
</div>  <script>  
// Music Player Toggle  
const bgMusic = document.getElementById("bgMusic");  
const musicBtn = document.getElementById("musicBtn");  
let isPlaying = false;  
  
// Set gentle default volume (30%)  
bgMusic.volume = 0.3;  
  
function toggleAudio() {  
  if (isPlaying) {  
    bgMusic.pause();  
    musicBtn.innerHTML = "🎵 Play Music";  
  } else {  
    bgMusic.play().catch(() => {});  
    musicBtn.innerHTML = "⏸️ Pause Music";  
  }  
  isPlaying = !isPlaying;  
}  
  
// Background Floating Particles  
const bg = document.getElementById("background");  
for(let i = 0; i < 35; i++){  
  const c = document.createElement("div");  
  c.className = "circle";  
  c.style.width = Math.random() * 80 + 20 + "px";  
  c.style.height = c.style.width;  
  c.style.left = Math.random() * 100 + "vw";  
  c.style.animationDuration = Math.random() * 10 + 8 + "s";  
  c.style.animationDelay = Math.random() * 5 + "s";  
  bg.appendChild(c);  
}  
  
// Step Switcher Helper  
function showStep(stepId) {  
  document.querySelectorAll('.container').forEach(el => el.style.display = 'none');  
  document.getElementById(stepId).style.display = 'block';  
}  
  
function startJourney(){  
  showStep('step2');  
  if(!isPlaying) toggleAudio();  
}  
  
// Letter Content and Typewriter Effect  
const letterText = `Hey Pihu, ❤️  
  
Happy Girlfriend's Day.  
  
I just wanted to say thank you. You've always been there for me, through the good days and the difficult ones. Because of you, I've grown into a better version of myself, and I'll always be grateful for that.  
  
No matter what happens or where life takes us, I'll always be there for you, just like you'been there for me.  
  
This little surprise may not be perfect, but every part of it was made with lots of care, just to make you smile.  
  
— Ur Tamato 🥀  
  
.-.. --- ...- . / -.-- --- ..- ❤️`;  
  
let letterIndex = 0;  
  
function openLetter(){  
  document.getElementById("envelopeSection").style.display = "none";  
  document.getElementById("letterContent").style.display = "block";  
  typeLetter();  
}  
  
function typeLetter(){  
  const area = document.getElementById("letterContent");  
  if(letterIndex < letterText.length){  
    area.innerHTML += letterText.charAt(letterIndex);  
    letterIndex++;  
    setTimeout(typeLetter, 30);  
  } else {  
    document.getElementById("nextBtn").style.display = "inline-block";  
  }  
}  
  
function giftPage(){  
  showStep('step3');  
}  
  
function puzzlePage(){  
  showStep('step4');  
}  
  
// Quiz Game Logic  
let attempts = 0;  
  
function checkAnswer(){  
  const ans = document.getElementById("answer").value.toLowerCase().trim();  
  const res = document.getElementById("result");  
  
  if(ans === "no one" || ans === "nobody"){  
    res.style.color = "#81c784";  
    res.innerHTML = "✅ Correct!<br><br><b>Exactly. No one ❤️</b>";  
    setTimeout(() => {  
      showStep('step5');  
      drawAxes();  
    }, 2000);  
  } else {  
    attempts++;  
    if(attempts >= 3){  
      res.style.color = "#ffb6d0";  
      res.innerHTML = "I love u more than anyone ❤️";  
      setTimeout(() => {  
        showStep('step5');  
        drawAxes();  
      }, 2500);  
    } else {  
      res.style.color = "#ff8a80";  
      res.innerHTML = "❌ Wrong answer.<br><span style='font-size:15px; color:#ffd6e7;'>Hint: Think again... ❤️</span>";  
    }  
  }  
}  
  
// Draw X and Y Axes on Canvas  
function drawAxes() {  
  const canvas = document.getElementById("heartCanvas");  
  const ctx = canvas.getContext("2d");  
  const w = canvas.width;  
  const h = canvas.height;  
  
  ctx.clearRect(0, 0, w, h);  
  
  // Axis styling  
  ctx.strokeStyle = "rgba(255, 255, 255, 0.25)";  
  ctx.lineWidth = 1;  
  
  // X Axis  
  ctx.beginPath();  
  ctx.moveTo(20, h / 2);  
  ctx.lineTo(w - 20, h / 2);  
  ctx.stroke();  
  
  // Y Axis  
  ctx.beginPath();  
  ctx.moveTo(w / 2, 20);  
  ctx.lineTo(w / 2, h - 20);  
  ctx.stroke();  
  
  // Axis Labels (X & Y)  
  ctx.fillStyle = "rgba(255, 255, 255, 0.4)";  
  ctx.font = "12px Poppins, sans-serif";  
  ctx.fillText("x", w - 15, h / 2 + 15);  
  ctx.fillText("y", w / 2 + 8, 18);  
}  
  
// Plotting the Heart Curve over the Axes  
function drawHeart(){  
  document.getElementById("drawBtn").style.display = "none";  
  const canvas = document.getElementById("heartCanvas");  
  const ctx = canvas.getContext("2d");  
  
  ctx.strokeStyle = "#ff4d88";  
  ctx.lineWidth = 3;  
  ctx.beginPath();  
  
  let t = 0;  
  const timer = setInterval(() => {  
    // Parametric heart curve mapping  
    const x = 16 * Math.pow(Math.sin(t), 3);  
    const y = 13 * Math.cos(t) - 5 * Math.cos(2*t) - 2 * Math.cos(3*t) - Math.cos(4*t);  
  
    const px = 175 + x * 8;  
    const py = 165 - y * 8;  
  
    if(t === 0){  
      ctx.moveTo(px, py);  
    } else {  
      ctx.lineTo(px, py);  
      ctx.stroke();  
    }  
  
    t += 0.04;  
  
    if(t >= Math.PI * 2){  
      clearInterval(timer);  
      setTimeout(() => {  
        showStep('step6');  
        heartRain();  
      }, 1200);  
    }  
  }, 25);  
}  
  
// Final Page Heart Rain Effect  
function heartRain(){  
  for(let i = 0; i < 50; i++){  
    const h = document.createElement("div");  
    h.innerHTML = "❤️";  
    h.style.position = "fixed";  
    h.style.left = Math.random() * 100 + "vw";  
    h.style.top = "-30px";  
    h.style.fontSize = (Math.random() * 20 + 18) + "px";  
    h.style.zIndex = "999";  
    document.body.appendChild(h);  
  
    h.animate([  
      { transform: "translateY(0px)", opacity: 1 },  
      { transform: "translateY(110vh)", opacity: 0 }  
    ], {  
      duration: 3000 + Math.random() * 3000,  
      iterations: 1,  
      fill: "forwards"  
    });  
  }  
}  
</script>  </body>  


