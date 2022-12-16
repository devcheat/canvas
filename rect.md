
## HTML canvas `rect()` Method
``` html
<canvas id="mc17" width="300" height="150" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc17");
        var ctx = c.getContext("2d");
        ctx.rect(20, 20, 150, 100);
        ctx.stroke();
</script>
```

## HTML canvas `clearRect()` Method
``` html
<canvas id="mc18" width="300" height="150" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc18");
        var ctx = c.getContext("2d");
        ctx.fillStyle = "red";
        ctx.fillRect(0, 0, 300, 150);
        ctx.clearRect(20, 20, 100, 50);
</script>
```

## HTML canvas `strokeRect()` Method
``` html
<canvas id="mc19" width="300" height="150" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc19");
        var ctx = c.getContext("2d");
        ctx.strokeRect(20, 20, 150, 100);
</script>
```

## HTML canvas `fillRect()` Method
``` html
<canvas id="mc20" width="300" height="150" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc20");
        var ctx = c.getContext("2d");
        ctx.fillRect(20, 20, 150, 100);
</script>
```
