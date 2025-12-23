<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>BnBatuu Partisi</title>

  <style>
    body {
      background: black;
      color: white;
      text-align: center;
      font-family: Arial;
      margin-top: 120px;
      overflow: hidden;
    }
    button {
      background: red;
      color: white;
      border: none;
      padding: 15px 25px;
      font-size: 20px;
      border-radius: 10px;
    }
    .confetti {
      position: fixed;
      width: 10px;
      height: 10px;
      top: -10px;
      animation: fall 3s linear infinite;
    }
    @keyframes fall {
      to {
        transform: translateY(100vh) rotate(360deg);
      }
    }
  </style>
</head>

<body>

<h1>BnBatuu 🔥</h1>
<p>Abone ol → Parti başlasın 🎉</p>

<button onclick="party()">BnBatuu Kanalına Gir</button>

<script>
function party() {
  window.open("https://www.youtube.com/@PrimeBatu-q9x", "_blank");

  for (let i = 0; i < 50; i++) {
    let c = document.createElement("div");
    c.className = "confetti";
    c.style.left = Math.random() * window.innerWidth + "px";
    c.style.background =
      ["red","yellow","blue","green","pink"][Math.floor(Math.random()*5)];
    c.style.animationDuration = (Math.random() * 2 + 1) + "s";
    document.body.appendChild(c);
  }
}
</script>

</body>
</html>
