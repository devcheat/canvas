# HTML canvas `bezierCurveTo()` Method
``` html
        <canvas id="mc23" width="300" height="150" style="border:1px solid #d3d3d3;">
                Your browser does not support the HTML5 canvas tag.</canvas>

<script>
    var c = document.getElementById("mc23");
    var ctx = c.getContext("2d");
    ctx.beginPath();
    ctx.moveTo(20, 20);
    ctx.bezierCurveTo(20, 100, 200, 100, 200, 20);
    ctx.stroke();
</script>
```
