 <!DOCTYPE html> 
 <html lang="es"> 
   <head> 
    <meta charset="UTF-8"> 
     <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
     <title>¿Quieres ser mi San Valentín</title>
     <style> 
       body {
         text-align: center; font-family: Arial, sans-serif; background-color: #ffebf0; 
       } 
       .container { 
         margin-top: 50px; 
       }
       h1
       { 
         color: #ff4081; font-size: 2em; 
       } 
       .buttons { 
         margin-top: 20px; 
       } 
       button {
         font-size: 1.2em; 
         padding: 10px 20px;
         margin: 10px; 
         border: none; 
         cursor: pointer; 
         border-radius: 5px; 
       } 
       .yes { 
         background-color: #ff4081;
         color: white;
       } 
       .no { 
         background-color: #ccc; 
         color: black;
         position: absolute;
       } 
     </style> 
   </head> 
   <body> 
     <div class="container">
       <h1>¿Quieres ser mi San Valentín? ❤️</h1> 
       <div class="buttons">
         <button class="yes" onclick="aceptar()">Sí</button> 
         <button class="no" onmouseover="moverNo()">No</button>
       </div> 
     </div> 
     
     <script> 
     function aceptar() { 
     alert("¡Sabía que dirías que sí! ❤️"); 
     } 
     function moverNo() {
     let botonNo = document.querySelector(".no"); 
     let x = Math.random() * 
(window.innerWidth - botonNo.offsetWidth); 
let y = Math.random() * (window.innerHeight - botonNo.offsetHeight); 
botonNo.style.left = x + "px"; 
botonNo.style.top = y + "px";
}
</script>
</body> 
</html> 

