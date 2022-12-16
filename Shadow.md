# Shadow 

## HTML canvas `shadowOffsetY` Property
> Draw a rectangle with a shadow placed 20 pixels below the rectangle's top position:
``` html
<canvas id="mc11" width="300" height="150" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc11");
        var ctx = c.getContext("2d");
        ctx.shadowBlur = 10;
        ctx.shadowOffsetY = 20;
        ctx.shadowColor = "black";
        ctx.fillStyle = "red";
        ctx.fillRect(20, 20, 100, 80);
</script>
```

## HTML canvas `shadowOffsetX` Property
``` html
<canvas id="mc12" width="300" height="150" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc12");
        var ctx = c.getContext("2d");
        ctx.shadowBlur = 10;
        ctx.shadowOffsetX = 20;
        ctx.shadowColor = "black";
        ctx.fillStyle = "red";
        ctx.fillRect(20, 20, 100, 80);
</script>
```

## HTML canvas `shadowColor` Property
``` html
<canvas id="mc13" width="300" height="150" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc13");
        var ctx = c.getContext("2d");
        ctx.shadowBlur = 20;
        ctx.fillStyle = "red";

        ctx.shadowColor = "black";
        ctx.fillRect(20, 20, 100, 80);

        ctx.shadowColor = "blue";
        ctx.fillRect(140, 20, 100, 80);
</script>
```

## HTML canvas `shadowBlur` Property
``` html
<canvas id="mc14" width="300" height="150" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc14");
        var ctx = c.getContext("2d");
        ctx.shadowBlur = 20;
        ctx.shadowColor = "black";
        ctx.fillStyle = "red";
        ctx.fillRect(20, 20, 100, 80);
</script>
```
