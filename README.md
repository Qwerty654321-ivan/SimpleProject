# SimpleProject slider jquery
<!DOCTYPE html>
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body>
    
    <img id="slider" src="http://www.sololearn.com/uploads/slider/1.jpg" width="200px" height="100px"/>
    
    <script src="https://code.jquery.com/jquery-3.4.1.js"></script>
         <script>
            
            var images =[
   'http://www.sololearn.com/uploads/slider/3.jpg',   
   'http://www.sololearn.com/uploads/slider/3.jpg',   
 'http://www.sololearn.com/uploads/slider/2.jpg',  
 'http://www.sololearn.com/uploads/slider/2.jpg',         'http://www.sololearn.com/uploads/slider/1.jpg',
 'http://www.sololearn.com/uploads/slider/1.jpg'];
              
            
       
            var img = $('img');
            var i = 0;
            var speed = 900;
    
     
            setInterval(function(){
            
            
                img.animate({
                    width:'toggle'
                },900);
                    
                  var slider = document.getElementById('slider');    
     i++;
     
     if(i >= images.length) {
        i = 0;
    }
    slider.src = images[i];     
       
            },speed);
            
        </script>
    </body>
</html>
