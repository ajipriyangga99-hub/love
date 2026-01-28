<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Love</title>

<style>
/* RESET */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html, body {
    width: 100%;
    height: 100%;
    background: radial-gradient(circle at top, #300000, #000);
    overflow: hidden;
    font-family: 'Segoe UI', sans-serif;
}

/* CENTER */
body {
    display: flex;
    justify-content: center;
    align-items: center;
}

/* CONTAINER */
#container {
    text-align: center;
}

/* EMOJI HEART */
#heart {
    font-size: 120px;
    animation: beat 1s infinite;
    filter: drop-shadow(0 0 25px red);
}

/* HEART BEAT */
@keyframes beat {
    0%   { transform: scale(1); }
    25%  { transform: scale(1.15); }
    50%  { transform: scale(1); }
    75%  { transform: scale(1.2); }
    100% { transform: scale(1); }
}

/* TEXT */
#text {
    margin-top: 20px;
    font-size: 28px;
    font-weight: bold;
    letter-spacing: 2px;
    color: #ff4d4d;
    text-shadow: 0 0 10px red;
    animation: glow 2s infinite alternate;
}

/* TEXT GLOW */
@keyframes glow {
    from { text-shadow: 0 0 5px red; }
    to   { text-shadow: 0 0 20px #ff0000; }
}

/* FLOATING HEARTS */
.floating {
    position: absolute;
    font-size: 24px;
    animation: floatUp 6s linear infinite;
    opacity: 0.8;
}

@keyframes floatUp {
    0% {
        transform: translateY(0) scale(1);
        opacity: 0;
    }
    20% { opacity: 1; }
    100% {
        transform: translateY(-800px) scale(1.5);
        opacity: 0;
    }
}
</style>
</head>

<body>

<div id="container">
    <div id="heart">❤️</div>
    <div id="text">I LOVE PUTRI SEPTIANA SARI</div>
</div>

<!-- FLOATING HEARTS -->
<script>
for (let i = 0; i < 20; i++) {
    const heart = document.createElement("div");
    heart.className = "floating";
    heart.innerHTML = "❤️";
    heart.style.left = Math.random() * 100 + "vw";
    heart.style.animationDelay = Math.random() * 6 + "s";
    heart.style.fontSize = (20 + Math.random() * 20) + "px";
    document.body.appendChild(heart);
}
</script>

</body>
</html>
