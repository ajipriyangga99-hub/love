<html lang="en">
<head>
<meta charset="UTF-8">
<title>Love</title>

<style>
/* RESET TOTAL */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    background: transparent;
}

html, body {
    width: 100%;
    height: 100%;
    background: black; /* GANTI ke transparent jika mau */
    overflow: hidden;
}

/* CENTER */
body {
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: monospace;
}

/* CONTAINER */
#container {
    text-align: center;
}

/* HEART */
#heart {
    white-space: pre;
    font-size: 16px;
    line-height: 16px;
    color: red;
    animation: beat 1s infinite;
    background: transparent;
}

/* ANIMATION */
@keyframes beat {
    0%   { transform: scale(1); }
    25%  { transform: scale(1.1); }
    50%  { transform: scale(1); }
    75%  { transform: scale(1.15); }
    100% { transform: scale(1); }
}

/* TEXT */
#text {
    margin-top: 15px;
    font-size: 24px;
    font-weight: bold;
    color: red;
    background: transparent;
}
</style>
</head>

<body>

<div id="container">
<pre id="heart">
      ♥♥     ♥♥      
   ♥♥♥♥♥♥♥♥♥♥♥♥♥
 ♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥
 ♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥
  ♥♥♥♥♥♥♥♥♥♥♥♥♥♥
    ♥♥♥♥♥♥♥♥♥♥♥
      ♥♥♥♥♥♥♥♥
        ♥♥♥♥♥
          ♥
</pre>

<div id="text">I LOVE PUTRI SEPTIANA SARI</div>
</div>

</body>
</html>
