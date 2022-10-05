
Just paste the JavaScript below into the address bar of any browser then press Enter, it makes all pictures on the current web page fly around like a snake when you move the pointer.
javascript:R=0; x1=.1; y1=.05; x2=.25; y2=.24; x3=1.6; y3=.24; x4=300; y4=200; x5=300; y5=200; var DI= document.getElementsByTagName("img"); DIL=DI.length; function A(){for(i=0; i<DIL; i++){DIS=DI[ i ].style; DIS.position='absolute'; DIS.left=Math.sin(R*x1+i*x2+x3)*x4+x5+"px"; DIS.top=Math.cos(R*y1+i*y2+y3)*y4+y5+"px"}R++}tag=setInterval('A()',5 );document.onmousedown=function(){clearInterval(tag);for(i=0; i<DIL; i++){DI[i].style.position="static";}}; void(0)
In the above JavaScript, you can change document.getElementsByTagName("img") to any HTML tag that you want to apply.

Here’s some another versions of this effect: javascript:R=0;x1=.1;y1=.05;x2=.25;y2=.24;x3=1.6;y3=.24;x4=300;y4=200;x5=300;y5=200;DI= document.images;DIL=DI.length;function A(){for(i=0; i<DIL; i++){DIS=DI[ i ].style;DIS.position='absolute' ;DIS.left=Math.sin(R*x1+ i*x2+x3)* x4+x5;DIS.top=Math.cos(R*y1+ i*y2+y3)* y4+y5;} R++;}setInterval('A()',5);void(0);
