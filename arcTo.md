# HTML canvas `arcTo()` Method
Create an arc between two tangents on the canvas:

| Parameter | Description                            |
| --------- | -------------------------------------- |
| x1        | The x-coordinate of the first tangent  |
| y1        | The y-coordinate of the first tangent  |
| x2        | The x-coordinate of the second tangent |
| y2        | The y-coordinate of the second tangent |
| r         | The radius of the arc                  |


```html
<canvas id="mc24" width="300" height="150" style="border:1px solid #d3d3d3;">
        Your browser does not support the HTML5 canvas tag.</canvas>

<script>
        var c = document.getElementById("mc24");
        var ctx = c.getContext("2d");
        ctx.beginPath();
        ctx.moveTo(20, 20); // Create a starting point
        ctx.lineTo(100, 20); // Create a horizontal line
        ctx.arcTo(150, 20, 150, 70, 50); // Create an arc
        ctx.lineTo(150, 120); // Continue with vertical line
        ctx.stroke(); // Draw it
</script>
```
