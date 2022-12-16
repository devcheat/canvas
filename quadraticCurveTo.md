# HTML canvas `quadraticCurveTo()` Method

## Definition and Usage
> The quadraticCurveTo() method adds a point to the current path by using the specified control points that represent a quadratic Bézier curve.
        
A quadratic Bézier curve requires two points. The first point is a control point that is used in the quadratic Bézier calculation and the second point is the ending point for the curve. The starting point for the curve is the last point in the current path. If a path does not exist, use the beginPath() and moveTo() methods to define a starting point.

``` javascript
Start point: moveTo(20,20)
Control point: quadraticCurveTo(20,100,200,20)
End point: quadraticCurveTo(20,100,200,20) 
```
| Parameter | Description                                  |
| --------- | -------------------------------------------- |
| `cpx`       | The x-coordinate of the Bézier control point |
| `cpy`       | The y-coordinate of the Bézier control point |
| `x`         | The x-coordinate of the ending point         |
| `y`         | The y-coordinate of the ending point         |

``` html
<canvas id="mc22" width="300" height="150" style="border:1px solid #d3d3d3;">
                Your browser does not support the HTML5 canvas tag.</canvas>

<script>
    var c = document.getElementById("mc22");
    var ctx = c.getContext("2d");
    ctx.beginPath();
    ctx.moveTo(20, 20);
    ctx.quadraticCurveTo(20, 100, 200, 20);
    ctx.stroke();
</script>
```
