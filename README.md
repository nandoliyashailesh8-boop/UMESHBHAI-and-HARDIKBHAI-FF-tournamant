<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>UMESHBHAI & Hardik Tournament</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body{
margin:0;
font-family:Arial,sans-serif;
background:#0b0b0b;
color:#fff;
}

/* HEADER */
header{
background:#ffb300;
color:#000;
padding:15px;
text-align:center;
font-size:22px;
font-weight:bold;
}

/* COMMON */
.section-title{
text-align:center;
color:#ffb300;
margin:25px 0 10px;
font-size:20px;
}

.container{
padding:15px;
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:20px;
}

/* CARD */
.card{
background:#111;
border-radius:15px;
box-shadow:0 0 15px #ffb300;
overflow:hidden;
text-align:center;
}
.card img{
width:100%;
height:auto;
display:block;
}
.card h3{color:#ffb300;margin:10px 0}
.card p{font-size:14px}

/* BUTTON */
.btn{
display:block;
margin:12px;
padding:12px;
background:#ffb300;
color:#000;
text-decoration:none;
border-radius:8px;
font-weight:bold;
}
.btn:hover{background:#ffd54f}

/* TIMER */
.timer{
font-size:18px;
margin:10px;
color:#00ffcc;
text-align:center;
}

/* PAYMENT */
.payment{
background:#111;
margin:20px;
padding:15px;
border-radius:15px;
box-shadow:0 0 15px #ffb300;
text-align:center;
}
.payment img{width:200px}

/* RULES */
.rules{
background:#111;
margin:20px;
padding:15px;
border-radius:15px;
font-size:14px;
line-height:1.6;
}

/* GALLERY */
.gallery{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(140px,1fr));
gap:10px;
padding:15px;
}
.gallery img{
width:100%;
border-radius:10px;
}

/* FOOTER */
footer{
text-align:center;
padding:15px;
font-size:13px;
opacity:0.8;
}
</style>
</head>

<body>

<header>🔥 UMESHBHAI & Hardik Tournament 🔥</header>

<div class="section-title">⏳ Match Starts In</div>
<div class="timer" id="timer">Loading...</div>

<div class="section-title">🎮 Available Matches</div>

<div class="container">

<div class="card">
<img src="https://picsum.photos/seed/solo/600/400" alt="Solo Match">
<h3>SOLO MATCH</h3>
<p>Entry Fee: ₹30</p>
<p>Prize: ₹500</p>
<a href="#payment" class="btn">JOIN NOW</a>
</div>

<div class="card">
<img src="https://picsum.photos/seed/duo/600/400" alt="Duo Match">
<h3>DUO MATCH</h3>
<p>Entry Fee: ₹50</p>
<p>Prize: ₹1000</p>
<a href="#payment" class="btn">JOIN NOW</a>
</div>

<div class="card">
<img src="https://picsum.photos/seed/squad/600/400" alt="Squad Match">
<h3>SQUAD MATCH</h3>
<p>Entry Fee: ₹100</p>
<p>Prize: ₹3000</p>
<a href="#payment" class="btn">JOIN NOW</a>
</div>

</div>

<div class="section-title">📜 Tournament Rules</div>
<div class="rules">
1️⃣ No hacks / cheats allowed<br>
2️⃣ Room ID WhatsApp par milegi<br>
3️⃣ Match start ke baad entry allow nahi<br>
4️⃣ Payment non-refundable<br>
5️⃣ Screenshot WhatsApp par bhejna compulsory
</div>

<div class="section-title">💰 Payment Method</div>
<div id="payment" class="payment">
<h3>UPI ID</h3>
<h2>Thakoru429@okicici</h2>

<img src="https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=upi://pay?pa=Thakoru429@okicici" alt="UPI QR">

<p>Google Pay • PhonePe • Paytm • BHIM</p>
<p>Payment ke baad screenshot WhatsApp par bheje</p>

<a class="btn" href="https://wa.me/918487801647?text=Payment%20Done%20for%20Tournament">
📲 Send Screenshot on WhatsApp
</a>
</div>

<div class="section-title">📸 Tournament Gallery</div>
<div class="gallery">
<img src="https://picsum.photos/seed/g1/300/200">
<img src="https://picsum.photos/seed/g2/300/200">
<img src="https://picsum.photos/seed/g3/300/200">
<img src="https://picsum.photos/seed/g4/300/200">
</div>

<footer>
© 2025 UMESHBHAI & Hardik Tournament | All Rights Reserved
</footer>

<!-- ✅ FIXED COUNTDOWN TIMER -->
<script>
let remainingTime = 60 * 60; // 1 hour
const timer = document.getElementById("timer");

const interval = setInterval(() => {
    let minutes = Math.floor(remainingTime / 60);
    let seconds = remainingTime % 60;

    seconds = seconds < 10 ? "0" + seconds : seconds;

    timer.innerHTML = minutes + " Minutes " + seconds + " Seconds";

    if (remainingTime <= 0) {
        clearInterval(interval);
        timer.innerHTML = "⏰ Match Started!";
    }

    remainingTime--;
}, 1000);
</script>

</body>
</html>
