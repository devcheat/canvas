# HTML canvas` isPointInPath()` Method
``` html
<canvas id="mc25" width="300" height="150" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc25");
        var ctx = c.getContext("2d");
        ctx.rect(20, 20, 150, 100);
        if (ctx.isPointInPath(20, 50)) {
                ctx.stroke();
        };
</script>
```
