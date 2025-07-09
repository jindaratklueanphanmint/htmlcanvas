# htmlcanvas
<!DOCTYPE html>
<html>
<body>

<canvas id="myCanvas" width="350" height="350" style="border:1px solid #d3d3d3;">
Your browser does not support the HTML canvas tag.</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
var n = 5;
for (let i = 1; i <n; i++) {
  ctx.moveTo(i/n*(c.width),0);
  ctx.lineTo(i/n*(c.width),c.height);
  ctx.stroke();
}

ctx.stroke();
</script>

</body>
</html>
