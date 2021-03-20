# 3D-Cube-rotation
....html....
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    <script src="script.js"></script>
    <div id="wrapD3Cube">
    <div id="D3Cube">
        <div id="side1"></div>
        <div id="side2"></div>
        <div id="side3"></div>
        <div id="side4"></div>
        <div id="side5"></div>
        <div id="side6"></div>
    </div>
</div>
  </body>
  </html>
  .....css.....
  #wrapD3Cube {
    width: 250px;
    height: 213px;
    margin: 20px auto;
}
#D3Cube {
    width: 150px;
    height: 150px;
    top: 80px;
    transform-style: preserve-3d;
    -moz-transform-style: preserve-3d;
    -webkit-transform-style: preserve-3d;
    transform: rotateX(-22deg) rotateY(-38deg) rotateZ(0deg);
    -moz-transform: rotateX(-22deg) rotateY(-38deg) rotateZ(0deg);
    -webkit-transform: rotateX(-22deg) rotateY(-38deg) rotateZ(0deg);
    margin: auto;
    position: relative;
    -moz-transform-style: preserve-3d;
    transform-style: preserve-3d;
    -webkit-transition: all 0.5s ease-in-out;
    transition: all 0.5s ease-in-out;
    -webkit-animation: cubeRotation 5s infinite; /* Safari 4.0 - 8.0 */
    animation: cubeRotation 5s infinite;
}
/* Safari 4.0 - 8.0 */
@-webkit-keyframes cubeRotation {
    0%   {	-webkit-transform: rotateX(-22deg) rotateY(-38deg) rotateZ(0deg);	}
    50%   {	-webkit-transform: rotateX(-22deg) rotateY(-128deg) rotateZ(0deg);	}
    100%   {	-webkit-transform: rotateX(-22deg) rotateY(-398deg) rotateZ(0deg);	}
}
/* Standard syntax */
@keyframes cubeRotation {
    0%   {	transform: rotateX(-22deg) rotateY(-38deg) rotateZ(0deg);	}
    50%   {	transform: rotateX(-22deg) rotateY(-238deg) rotateZ(0deg);	}
    100%   {	transform: rotateX(-22deg) rotateY(-398deg) rotateZ(0deg);	}
}
#D3Cube > div {
    position: absolute;
    -webkit-transition: all 0.5s ease-in-out;
    transition: all 0.5s ease-in-out;
    width: 150px;
    height: 150px;
    float: right;
    overflow: hidden;
	opacity: 0.90;
}
#side1 {
    transform: rotatex(90deg) translateX(0px) translateY(0px) translateZ(56px);
    -moz-transform: rotatex(90deg) translateX(0px) translateY(0px) translateZ(56px);
    -webkit-transform: rotatex(90deg) translateX(0px) translateY(0px) translateZ(56px);
	background-color: aquamarine;
}
#side2 {
    transform: rotateY(-90deg) translateX(0px) translateY(0px) translateZ(56px);
    -moz-transform: rotateY(-90deg) translateX(0px) translateY(0px) translateZ(56px);
    -webkit-transform: rotateY(-90deg) translateX(0px) translateY(0px) translateZ(56px);
	background-color: lightpink;
}
#side3 {
    transform: translateX(0px) translateY(0px) translateZ(56px);
    -moz-transform: translateX(0px) translateY(0px) translateZ(56px);
    -webkit-transform: translateX(0px) translateY(0px) translateZ(56px);
	background-color: sienna;
}
#side4 {
    transform: rotateY(90deg) translateX(0px) translateY(0px) translateZ(56px);
    -moz-transform: rotateY(90deg) translateX(0px) translateY(0px) translateZ(56px);
    -webkit-transform: rotateY(90deg) translateX(0px) translateY(0px) translateZ(56px);
	background-color: yellow;
}
#side5 {
    transform: rotateY(180deg) translateX(0px) translateY(0px) translateZ(56px);
    -moz-transform: rotateY(180deg) translateX(0px) translateY(0px) translateZ(56px);
    -webkit-transform: rotateY(180deg) translateX(0px) translateY(0px) translateZ(56px);
	background-color: slateblue;
}
#side6 {
    transform: rotateX(-90deg) translateX(0px) translateY(0px) translateZ(56px);
    -moz-transform: rotateX(-90deg) translateX(0px) translateY(0px) translateZ(56px);
    -webkit-transform: rotateX(-90deg) translateX(0px) translateY(0px) translateZ(56px);
	background-color: magenta;
}
