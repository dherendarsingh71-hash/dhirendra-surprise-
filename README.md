# dhirendra-surprise-

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>For Ritika 💗</title>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  min-height: 100vh;
  background: linear-gradient(135deg,#ffe0eb,#fff0f5,#f8cadd);
  font-family: Georgia, serif;
  color: #914765;
  text-align: center;
  padding: 25px 15px;
  overflow-x: hidden;
}

.card {
  max-width: 440px;
  margin: 30px auto;
  background: rgba(255,255,255,.82);
  padding: 30px 22px;
  border-radius: 28px;
  box-shadow: 0 10px 40px #bd6e9233;
}

.flower {
  font-size: 65px;
  animation: float 2s infinite;
}

h1 {
  color: #dc6694;
  margin: 15px 0;
}

h2 {
  color: #d46b92;
  margin: 20px 0 10px;
}

p {
  line-height: 1.8;
  margin: 12px 0;
}

.section {
  background: #fff0f5;
  padding: 18px;
  border-radius: 20px;
  margin: 20px 0;
}

button {
  border: none;
  padding: 13px 20px;
  margin: 7px;
  border-radius: 30px;
  background: #e77da5;
  color: white;
  font-size: 15px;
  cursor: pointer;
}

button:hover {
  background: #c94f7e;
}

#message {
  margin-top: 20px;
  min-height: 65px;
  color: #c04e7c;
  font-weight: bold;
  line-height: 1.7;
}

.hidden {
  display: none;
}

.heart {
  position: fixed;
  bottom: -30px;
  pointer-events: none;
  animation: rise 5s linear forwards;
}

@keyframes float {
  50% {transform: translateY(-10px);}
}

@keyframes rise {
  to {
    transform: translateY(-110vh) rotate(360deg);
    opacity: 0;
  }
}
</style>
</head>

<body>

<div class="card">

<div class="flower">🌷</div>

<h1>Hey Ritika! 💗</h1>

<p>
I made a little corner of happiness
just for you. 🥹
</p>

<p>
Because even on your not-so-good days,
you deserve a little extra love.
</p>

<div class="section">
<h2>First of all, take care! 🧸</h2>

<p>🍫 Eat your favourite chocolate.</p>
<p>☕ Have a warm drink if it feels comforting.</p>
<p>💧 Stay hydrated.</p>
<p>🛌 Give yourself some rest.</p>
<p>🌸 Don't be too hard on yourself.</p>
</div>

<h2>Your happiness menu ✨</h2>

<p>Choose anything you need right now!</p>

<button onclick="show('hug')">Virtual Hug 🤗</button>
<button onclick="show('chocolate')">Chocolate 🍫</button>
<button onclick="show('smile')">Make me smile 🌷</button>
<button onclick="show('love')">Secret message 💌</button>

<div id="message"></div>

<div class="section">
<h2>A little reminder ❤️</h2>

<p>
You don't have to smile all the time.
You don't have to pretend you're okay.
It's okay to rest, complain, laugh,
or do absolutely nothing.
</p>

<p>
Just remember, you're precious.
</p>
</div>

<button onclick="confession()">
One last thing... 🥺
</button>

<div id="secret" class="hidden section">
<h2>Ritika, listen... 💗</h2>

<p>
I don't know how to explain this,
but talking to you makes ordinary
days a little more special.
</p>

<p>
Maybe you're just my best friend...
or maybe my heart has a slightly
different opinion. 🙈
</p>

<p>
Whatever it is, I genuinely want
to see you happy.
</p>

<h2>Keep smiling, pretty girl! 🌷</h2>
</div>

<p style="margin-top:25px;font-size:13px;">
Made with extra care, just for Ritika ♡
<br>
From someone who loves your smile ❤️
</p>

</div>

<script>

function show(type) {

const messages = {
hug: "Come hereee! Biggest virtual hug for you! 🤗💗",
chocolate: "If I could, I'd bring you a whole box of chocolates right now! 🍫",
smile: "Reminder: You're beautiful, you're special and you deserve happiness! 🌷",
love: "Some people unknowingly become someone's favourite notification. Guess who? 🙈❤️"
};

document.getElementById("message").innerHTML =
messages[type];
}

function confession() {
document.getElementById("secret").style.display = "block";
document.getElementById("secret").scrollIntoView({
behavior: "smooth"
});
}

function createHeart() {
let heart = document.createElement("div");
heart.className = "heart";
heart.innerHTML = ["💗","💕","🌸","✨"][Math.floor(Math.random()*4)];
heart.style.left = Math.random()*100+"vw";
heart.style.fontSize = "22px";
document.body.appendChild(heart);
setTimeout(() => heart.remove(),5000);
}

setInterval(createHeart,600);

</script>

</body>
</html>
