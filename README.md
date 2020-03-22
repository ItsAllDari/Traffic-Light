# Traffic-Light
<!DOCTYPE html>
<html lang="en" >
<head>
  <meta charset="UTF-8">
  
  <link rel="stylesheet" href="./style.css">

</head>
<body>
<!-- partial:index.partial.html -->
<div id="controlPanel">
  <h1 id="stopButton" class="button">Stop</h1>
  <h1 id="slowButton" class="button">Slow</h1>
  <h1 id="goButton" 
      class="button">Go</h1>
</div>
<div id="traffic-light">
  <div id="stopLight" class="bulb"></div>
  <div id="slowLight" class="bulb"></div>
  <div id="goLight" class="bulb"></div>
</div>
<!-- partial -->
  <script src='https://cdnjs.cloudflare.com/ajax/libs/jquery/2.1.3/jquery.min.js'></script><script  src="./script.js"></script>

</body>
</html>

document.getElementById('stopButton').onclick = illuminateRed;
document.getElementById('slowButton').onclick = illuminateYellow;
document.getElementById('goButton').onclick= illuminateGreen;

function illuminateRed() {
  clearLights();
  document.getElementById('stopLight').style.backgroundColor = "red";
}

function illuminateYellow() {
  clearLights();
  document.getElementById('slowLight').style.backgroundColor = "yellow";
}

function illuminateGreen() {
  clearLights();
  document.getElementById('goLight').style.backgroundColor = "green";
}

function clearLights() {
  document.getElementById('stopLight').style.backgroundColor = "black";
  document.getElementById('slowLight').style.backgroundColor = "black";
  document.getElementById('goLight').style.backgroundColor = "black";
}
