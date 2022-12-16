# Draw a Circle
Define a circle with the arc() method. Then use the stroke() method to actually draw the circle:

``` html
<canvas id="mc03" width="200" height="100" style="border:1px solid #d3d3d3;background:#ffffff;">
        Your browser does not support the HTML5 canvas tag.
</canvas>
<script>
    var c = document.getElementById("mc03");
    var canvOK = 1;
    try {
        c.getContext("2d");
    } 
    catch (er) 
    {
        canvOK = 0;
    }

    if (canvOK == 1) {
        var ctx = c.getContext("2d");
        ctx.beginPath();
        ctx.arc(95, 50, 40, 0, 2 * Math.PI);
        ctx.stroke();
    }
</script>

```
