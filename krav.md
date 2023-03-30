Let themusic = new Audio ("fjdklfjdkjf");
let reload = new audio (ksdfjdsfjs);

   fill("green");
   rectangle(5,5,totalWidth-10,totalHeight-10,"black");

   var player={x:100, y:100, size: 5, xSpeed: 5, ySpeed: 0 };
   var wplayer={x:800, y:200, size: 5, xSpeed: -5, ySpeed: 0 };
   function update(){

      with(player)
      {
    rectangle(x,y,size,size,"green");
    x += xSpeed;
    y +=ySpeed;

    if (keyboard.w){ySpeed =-5;xSpeed = 0;}
    
    if (keyboard.s){ ySpeed = 5; xSpeed =0;}

    if (keyboard.a){ xSpeed = -5;  ySpeed =0;}

    if (keyboard.d){xSpeed = 5; ySpeed =0;}
 
    if (getPixel(x,y) .green !=0)
    stopUpdate();
    }

    with(wplayer)
      {

    rectangle(x,y,size,size,"orange");
    x += xSpeed;
    y +=ySpeed;

    if (keyboard.up){ySpeed =-5;xSpeed = 0;}
    
    if (keyboard.down){ ySpeed = 5; xSpeed =0;}

    if (keyboard.left){ xSpeed = -5;  ySpeed =0;}

    if (keyboard.right){xSpeed = 5; ySpeed =0;}
    if (getPixel(x,y) .green !=0)
    stopUpdate();
      }
    }
    
    
    
    

  
</script> 

</html>