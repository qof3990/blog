<p><canvas id="canvas1" width="580" height="200"></canvas></p>
<script type="text/javascript">
                              var canvas1=document.getElementById("canvas1");
                              var ctx=canvas1.getContext("2d");
                              ctx.lineWidth=1;
                              ctx.strokeStyle="#d3d3d3";
                              var x0=50,y0=0,x1=100,y1=100,x2=200,y2=100,r=0,x3=0,y3=0;
                              for (var i=0;i<72;i++){
                              r=r+Math.PI/36;
                              x2=x0+x1+100*Math.cos(r);
                              y2=y0+y1+100*Math.sin(r);
                              x3=x0+x1*3-100*Math.cos(r);
                              y3=y0+y1-100*Math.sin(r);
                              ctx.moveTo(x3,y3);
                              ctx.lineTo(x2,y2);
                              }
                              ctx.stroke();
                          </script>
