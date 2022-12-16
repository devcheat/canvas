# Drawing Text on the Canvas 
> To draw text on a canvas, the most important property and methods are:

- font - defines the font properties for the text
- fillText(text,x,y) - draws "filled" text on the canvas
- strokeText(text,x,y) - draws text on the canvas (no fill)

## Using `fillText()`

``` html
<canvas id="mc08" width="200" height="100" style="border:1px solid #d3d3d3;">
        Your browser does not support the canvas element.
</canvas>

<script>
    var canvas = document.getElementById("mc08");
    var ctx = canvas.getContext("2d");
    ctx.font = "30px Arial";
    ctx.shadowBlur = 40;
    ctx.shadowOffsetY = 0;
    ctx.shadowOffsetX = 0;
    ctx.shadowColor = "#53FFFF";
    ctx.fillText("Hello World", 10, 50);
</script>

```
## Using `strokeText()`
> some

``` html
<canvas id="mc09" width="200" height="100" style="border:1px solid #d3d3d3;">
        Your browser does not support the canvas element.
</canvas>

<script>
    var canvas = document.getElementById("mc09");
    var ctx = canvas.getContext("2d");
    ctx.font = "30px Arial";
    ctx.strokeText("Hello World", 10, 50);
</script>
```

## Add Color and Center Text
``` html
<canvas id="mc10" width="300" height="200" style="border:1px solid #d3d3d3;">
        Your browser does not support the canvas element.
</canvas>

<script>
        var canvas = document.getElementById("mc10");
        var ctx = canvas.getContext("2d");
        ctx.font = "30px Comic Sans MS";
        ctx.fillStyle = "red";
        ctx.textAlign = "center";
        ctx.fillText("Hello World", canvas.width / 2, canvas.height / 2);
</script>
```
