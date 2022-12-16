## Draw a Circle and make it glow
Use the shadow attribute for blur
``` html
<canvas id="mc04" width="400" height="200" 
style="border:1px solid #d3d3d3;background:#ffffff;">
        Your browser does not support the HTML5 canvas tag.
</canvas>
<script>
var c = document.getElementById("mc04");
var canvOK = 1;
try {
    c.getContext("2d");
} 
catch (er) {
    canvOK = 0;
}

if (canvOK == 1) {
    var ctx = c.getContext("2d");
    ctx.fillStyle = "black";
    ctx.fillRect(0, 0, 400, 200);
    ctx.beginPath();
    ctx.arc(95, 50, 40, 0, 2 * Math.PI);
    ctx.arc(195, 50, 10, 0, 2 * Math.PI);
    ctx.shadowBlur = 40;
    ctx.shadowOffsetY = 0;
    ctx.shadowOffsetX = 0;
    ctx.shadowColor = "#53FFFF";
    //ctx.stroke();
    // Create gradient
    var grd = ctx.createRadialGradient(75, 50, 5, 90, 60, 100);
    grd.addColorStop(0, "#53FFFF");
    grd.addColorStop(1, "#DBFFFF");

    // Fill with gradient
    ctx.fillStyle = grd;
    //ctx.fillStyle = "#99FFFF";
    ctx.fill();
}
</script>
```
