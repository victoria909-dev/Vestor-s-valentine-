# Vestor's-valentine-
<html>
<head>
<title>Happy Valentine Vestor ❤️</title>
<style>
body {
  background: linear-gradient(to bottom, #ffb6c1, #ffe4e1);
  text-align: center;
  font-family: 'Comic Sans MS', cursive;
  padding: 20px;
  overflow-x: hidden;
}

h1 {
  color: #b30000;
  font-size: 40px;
}

p {
  font-size: 20px;
  color: #4d0000;
}

.box {
  background: white;
  padding: 25px;
  border-radius: 25px;
  box-shadow: 0px 0px 15px pink;
  max-width: 700px;
  margin: auto;
  position: relative;
  z-index: 2;
}

.heart {
  font-size: 40px;
}

/* Floating hearts animation */
.heart-float {
  position: absolute;
  font-size: 20px;
  animation: float 8s linear infinite;
}

@keyframes float {
  0% {transform: translateY(100vh) translateX(0);}
  50% {transform: translateY(50vh) translateX(50px);}
  100% {transform: translateY(-10vh) translateX(-50px);}
}

#hearts-container {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 1;
}

/* Image styling */
.love-photo {
  max-width: 90%;
  border-radius: 20px;
  margin: 15px 0;
  box-shadow: 0 0 10px #ff9999;
}

/* 10 reasons list styling */
ul {
  text-align: left;
  display: inline-block;
  font-size: 18px;
  color: #990000;
  margin-top: 10px;
}
</style>
</head>

<body>

<!-- Background Music (Offline Ready) -->
<audio autoplay loop>
  <source src="valentine-music.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>

<!-- Floating hearts container -->
<div id="hearts-container"></div>

<div class="box">
<h1>Happy Valentine, Vestor ❤️</h1>
<div class="heart">💖💘💞</div>

<p>Hi babe 🥺</p>

<p>I just want you to know that you make me really happy.</p>

<p>Thank you for supporting me in the ways you can, even when things are not easy.  
And I’m sorry if I’ve ever been ungrateful in any way 😔.</p>

<p>I’m really grateful to have you in my life, and I appreciate how you always make sure I’m comfortable  
(even though you make sure everyone is comfortable 😏, you’re the only special person to me).</p>

<p>Thank you for loving me even on the days I’m hard to love, and for being patient with my moods and soft heart.</p>

<p>I may not have money for gifts this year, but I do have feelings, prayers, wishes, love,  
and this little website made just for you 🥺💖</p>

<h2>📸 A Special Memory</h2>
<img src="https://i.imgur.com/7Y5O2YX.jpg" alt="Us Together" class="love-photo">

<h2>💌 10 Reasons I Love You</h2>
<ul>
<li>You make me laugh even when I’m upset 😄</li>
<li>You support me in ways big and small 🙏</li>
<li>You notice the little things about me 💕</li>
<li>You’re kind, patient, and understanding 🥰</li>
<li>You make me feel safe and comfortable 😌</li>
<li>You believe in me even when I doubt myself 💪</li>
<li>You’re my favorite person to talk to 📞</li>
<li>You have a heart that loves unconditionally ❤️</li>
<li>You make everyday brighter 🌞</li>
<li>Simply because YOU are YOU, and that’s perfect for me 😭💖</li>
</ul>

<p><b>Happy Valentine’s Day, my favorite person 💕</b></p>

<p>From: Your girlfriend (trying very hard not to be shy calling you babe 😭😂)</p>

<div class="heart">❤️❤️❤️</div>
</div>

<script>
// Function to create floating hearts with random colors
function createHeart() {
  const heart = document.createElement('div');
  heart.className = 'heart-float';
  heart.style.left = Math.random() * window.innerWidth + 'px';
  heart.style.fontSize = 20 + Math.random() * 20 + 'px';
  
  // Random color: pink, red, purple
  const colors = ['#ff4d6d','#ff99c8','#cc66ff'];
  heart.style.color = colors[Math.floor(Math.random() * colors.length)];
  
  // Random animation speed
  heart.style.animationDuration = 4 + Math.random() * 6 + 's';
  heart.innerText = '💖';
  document.getElementById('hearts-container').appendChild(heart);

  // Remove heart after animation
  setTimeout(() => {
    heart.remove();
  }, 10000);
}

// Create hearts every 400ms
setInterval(createHeart, 400);
</script>

</body>
</html>
