<!DOCTYPE html>
<html lang="ar">
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta charset="UTF-8">
  <title>Domino Web</title>
  <style>
    body {
      background: #121212;
      color: white;
      font-family: Arial;
      text-align: center;
    }
    .tile {
      display: inline-block;
      border: 2px solid white;
      padding: 10px;
      margin: 5px;
      cursor: pointer;
    }
  </style>
</head>
<body>

<h1>🀄 Domino Web</h1>
<p>اختر بلاطة للعب</p>

<div id="player"></div>

<script>
  const tiles = ["6|6","6|5","5|5","4|3","2|1"];

  const playerDiv = document.getElementById("player");

  tiles.forEach(t => {
    const d = document.createElement("div");
    d.className = "tile";
    d.innerText = t;
    d.onclick = () => alert("لعبت البلاطة " + t);
    playerDiv.appendChild(d);
  });
</script>

</body>
</html>
