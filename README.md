# Parallax-1 is the basic website i have made just to show you how eventListners work when we scroll on the screen ,to achieving this effect we have to add a javascript in our HTML5 

**STEP-1**  ***first of all define all variables on which we are adding the effect***
 <script>
        let stars= document.getElementById('stars');
        let moon= document.getElementById('moon');
        let mountains_behind= document.getElementById('mountains_behind');
        let text= document.getElementById('text');
        let btn= document.getElementById('btn');
        let mountains_front= document.getElementById('mountains_front');
        let header=document.querySelector('header');
  
STEP-2      ***now add window.addEventListner and inside it define the property "scroll" ***
  
  
        window.addEventListener('scroll', function(){
            let value=window.scrollY;
            stars.style.left= value * 0.2 +'px';
            moon.style.top= value * 1 +'px';
            mountains_behind.style.marginTop= value * 0.9 +'px';
            mountains_front.style.marginTop= value * 0 +'px';
            text.style.marginRight= value * 3 +'px';
            text.style.marginTop= value * 0.5 +'px';
            btn.style.marginTop= value * 0.5 +'px';
            header.style.marginTop= value* 0.9 +'px';
        })
    </script>
