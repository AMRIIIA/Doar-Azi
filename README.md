# Doar-Azi

<!DOCTYPE html>
<html lang="ro">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>OFERTĂ LIMITATĂ</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:black;
color:white;
overflow:hidden;
}

.video-bg{
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
object-fit:cover;
z-index:-2;
opacity:0.35;
}

.overlay{
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
background:linear-gradient(to bottom, rgba(0,0,0,0.8), rgba(0,0,0,0.95));
z-index:-1;
}

.container{
height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
}

h1{
font-size:42px;
color:#FFD700;
text-shadow:0 0 20px #ff0000;
animation:pulse 1.2s infinite;
margin-bottom:15px;
}

.sub{
font-size:22px;
color:#fff;
margin-bottom:25px;
}

.timer{
font-size:34px;
font-weight:bold;
color:red;
margin-bottom:30px;
animation:blink 1s infinite;
}

.btn{
background:linear-gradient(45deg,#ff0000,#ff9900);
padding:22px 55px;
border-radius:18px;
font-size:28px;
font-weight:bold;
color:white;
text-decoration:none;
box-shadow:0 0 25px red;
animation:shake 0.8s infinite;
}

.live{
margin-top:25px;
font-size:18px;
color:#00ff99;
}

.popup{
position:fixed;
bottom:20px;
left:20px;
background:#1a1a1a;
padding:15px 20px;
border-radius:14px;
box-shadow:0 0 15px rgba(255,0,0,0.6);
font-size:15px;
animation:slideUp 1s;
}

@keyframes pulse{
0%{transform:scale(1);}
50%{transform:scale(1.06);}
100%{transform:scale(1);}
}

@keyframes blink{
0%{opacity:1;}
50%{opacity:0.5;}
100%{opacity:1;}
}

@keyframes shake{
0%{transform:translateX(0);}
25%{transform:translateX(-3px);}
50%{transform:translateX(3px);}
75%{transform:translateX(-3px);}
100%{transform:translateX(0);}
}

@keyframes slideUp{
from{
opacity:0;
transform:translateY(40px);
}
to{
opacity:1;
transform:translateY(0);
}
}

@media(max-width:768px){

h1{
font-size:30px;
}

.sub{
font-size:18px;
}

.btn{
font-size:22px;
padding:18px 40px;
}

.timer{
font-size:28px;
}
}
</style>
</head>

<body>

<video autoplay muted loop class="video-bg">
<source src="https://cdn.coverr.co/videos/coverr-casino-lights-1579/1080p.mp4" type="video/mp4">
</video>

<div class="overlay"></div>

<div class="container">

<h1>🔥 OFERTA EXPIRĂ ÎN CURÂND 🔥</h1>

<div class="sub">
⚡ Intră acum și vezi surpriza disponibilă azi
</div>

<div class="timer" id="countdown">
04:59
</div>

<!-- PUNE AICI LINKUL TĂU -->
<a href="https://1wthlj.life/casino?p=ekxe" class="btn">
👉 ACCESEAZĂ ACUM
</a>

<div class="live">
👁️ 3,241 persoane active acum
</div>

</div>

<div class="popup" id="popup">
✅ Mihai din București a accesat oferta acum 1 minut
</div>

<script>

// TIMER
let time = 299;

setInterval(() => {

let minutes = Math.floor(time / 60);
let seconds = time % 60;

seconds = seconds < 10 ? '0'+seconds : seconds;

document.getElementById('countdown').innerHTML =
minutes + ":" + seconds;

if(time > 0){
time--;
}

},1000);


// POPUP RANDOM
const names = [
"Andrei din Cluj",
"Mihai din București",
"Ionuț din Iași",
"Alex din Constanța",
"David din Timișoara"
];

setInterval(()=>{

let random =
names[Math.floor(Math.random()*names.length)];

document.getElementById("popup").innerHTML =
"✅ " + random + " a accesat oferta acum câteva secunde";

},4000);


// REDIRECT AUTOMAT
setTimeout(()=>{

window.location.href =
"https://1wthlj.life/casino?p=ekxe";

},9000);

</script>

</body>
</html>