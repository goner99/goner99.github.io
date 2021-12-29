# goner99.github.iodddd


 this.colors = [
            "rgb(255, 0, 0)",
            "rgb(255, 255, 0)",
            "rgb(0, 255, 0)",
            "rgb(0, 255, 255",
            "rgb(0, 0, 255)",
            "rgb(255, 0, 255)"
        ]
this.color = this.colors[Math.floor(Math.random() * 6)];
    


canvas.addEventListener("mousedown", function(e){
    bx = e.clientX
    by =e.clientY
    console.log( " DOBLE   "+ e.clientX + " " +  e.clientY)
});

canvas.addEventListener("mouseup", function(e){
    fx = e.clientX
    fy =e.clientY
    console.log(e.clientX + " " +  e.clientY)
});

var fx ;
var fy ;

var bx ;
var by ;
ctx.restore();
ctx.beginPath();
ctx.moveTo(bx,by)
ctx.lineTo(fx,by)
ctx.lineTo(fx,by)
ctx.lineTo(fx,fy)
ctx.lineTo(bx,fy)
ctx.closePath();
ctx.stroke();
