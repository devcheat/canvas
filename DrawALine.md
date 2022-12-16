# Draw a line
Use the `lineTo()` function to draw
``` html
<canvas id="mc05" width="200" height="100" style="border:1px solid #d3d3d3;">
        Your browser does not support the canvas element.
</canvas>

<script>
    var canvas = document.getElementById("mc05");
    var ctx = canvas.getContext("2d");
    ctx.moveTo(0, 0);
    ctx.lineTo(200, 100);
    ctx.stroke();
</script>
```
