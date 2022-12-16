
# Transformations 

## HTML canvas `scale()` Method
> The scale() method scales the current drawing, bigger or smaller.
        
Note: If you scale a drawing, all future drawings will also be scaled. The positioning will also be scaled. If you scale(2,2);
drawings will be positioned twice as far from the left and top of the canvas as you specify.

``` html        
<canvas id="mc26" width="300" height="150" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc26");
        var ctx = c.getContext("2d");

        ctx.strokeRect(5, 5, 25, 15);
        ctx.scale(2, 2);
        ctx.strokeRect(5, 5, 25, 15);
</script>
```

## HTML canvas `rotate()` Method
> To calculate from degrees to radians: degrees*Math.PI/180. Example: to rotate 5 degrees, specify the following: 5x*Math.PI/180

``` html
<canvas id="mc27" width="300" height="150" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc27");
        var ctx = c.getContext("2d");
        ctx.rotate(20 * Math.PI / 180);
        ctx.fillRect(50, 20, 100, 50);
</script>
```
## HTML canvas `transform()` Method
Notice that each time you call transform(), it builds on the previous transformation matrix:
``` html
<canvas id="mc28" width="300" height="150" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc28");
        var ctx = c.getContext("2d");

        ctx.fillStyle = "yellow";
        ctx.fillRect(0, 0, 250, 100)

        ctx.transform(1, 0.5, -0.5, 1, 30, 10);
        ctx.fillStyle = "red";
        ctx.fillRect(0, 0, 250, 100);

        ctx.transform(1, 0.5, -0.5, 1, 30, 10);
        ctx.fillStyle = "blue";
        ctx.fillRect(0, 0, 250, 100);
</script>
```

## HTML canvas `translate()` Method
Draw a rectangle in position (10,10), set new (0,0) position to (70,70). Draw same rectangle again (notice that the rectangle
                now starts in position (80,80):
``` html
<canvas id="mc29" width="300" height="150" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc29");
        var ctx = c.getContext("2d");
        ctx.fillRect(10, 10, 100, 50);
        ctx.translate(70, 70);
        ctx.fillRect(10, 10, 100, 50);
</script>
```

## HTML canvas `textAlign` Property
Create a red line in position 150. Position 150 is the anchor point for all the text defined in the example below. Study the effect of each textAlign property value:

``` html
<canvas id="mc30" width="300" height="200" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc30");
        var ctx = c.getContext("2d");

        // Create a red line in position 150
        ctx.strokeStyle = "red";
        ctx.moveTo(150, 20);
        ctx.lineTo(150, 170);
        ctx.stroke();

        ctx.font = "15px Arial";

        // Show the different textAlign values
        ctx.textAlign = "start";
        ctx.fillText("textAlign=start", 150, 60);
        ctx.textAlign = "end";
        ctx.fillText("textAlign=end", 150, 80);
        ctx.textAlign = "left";
        ctx.fillText("textAlign=left", 150, 100);
        ctx.textAlign = "center";
        ctx.fillText("textAlign=center", 150, 120);
        ctx.textAlign = "right";
        ctx.fillText("textAlign=right", 150, 140);
</script>
```

## HTML canvas `textBaseline` Property
``` html
<canvas id="mc31" width="400" height="200" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc31");
        var ctx = c.getContext("2d");

        //Draw a red line at y=100
        ctx.strokeStyle = "red";
        ctx.moveTo(5, 100);
        ctx.lineTo(395, 100);
        ctx.stroke();

        ctx.font = "20px Arial"

        //Place each word at y=100 with different textBaseline values
        ctx.textBaseline = "top";
        ctx.fillText("Top", 5, 100);
        ctx.textBaseline = "bottom";
        ctx.fillText("Bottom", 50, 100);
        ctx.textBaseline = "middle";
        ctx.fillText("Middle", 120, 100);
        ctx.textBaseline = "alphabetic";
        ctx.fillText("Alphabetic", 190, 100);
        ctx.textBaseline = "hanging";
        ctx.fillText("Hanging", 290, 100);
</script>
```
## HTML canvas `fillText()` Method
``` html
<canvas id="mc32" width="300" height="150" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc32");
        var ctx = c.getContext("2d");

        ctx.font = "20px Georgia";
        ctx.fillText("Hello World!", 10, 50);

        ctx.font = "30px Verdana";
        // Create gradient
        var gradient = ctx.createLinearGradient(0, 0, c.width, 0);
        gradient.addColorStop("0", "magenta");
        gradient.addColorStop("0.5", "blue");
        gradient.addColorStop("1.0", "red");
        // Fill with gradient
        ctx.fillStyle = gradient;
        ctx.fillText("Big smile!", 10, 90);
</script>
```

## HTML canvas `globalAlpha` Property
``` html
<canvas id="mc33" width="300" height="150" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc33");
        var ctx = c.getContext("2d");
        ctx.fillStyle = "red";
        ctx.fillRect(20, 20, 75, 50);

        //Turn transparency on
        ctx.globalAlpha = 0.2;
        ctx.fillStyle = "blue";
        ctx.fillRect(50, 50, 75, 50);
        ctx.fillStyle = "green";
        ctx.fillRect(80, 80, 75, 50);
</script>
```
