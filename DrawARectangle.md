# Draw a Rectangle
Drawing a rectangle
``` html
<canvas id="mc02" width="200" height="100" style="border:1px solid #c3c3c3;">
        Your browser does not support the canvas element.
</canvas>

<script>
    var canvas = document.getElementById("mc02");
    var ctx = canvas.getContext("2d");
    ctx.fillStyle = "#FF0000";
    ctx.fillRect(0, 0, 150, 75);
</script>
```
