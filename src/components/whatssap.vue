<template>
  



<!-- partial:index.partial.html -->
<div class="cotenido">
    <input type="checkbox" id="btn-mas">
    <div class="redes">
      <div class="encabezado">
       <b>¡Queremos Escucharte! Solicita tu primera cita online. ¡Estmos para ayudarte!</b>
      </div>
      <div class="agentes">
        <ul>
          <li><a href="" target="_blank"><i class="fa-solid fa-headset"></i>Sebastian</a></li>
        </ul>
        
      </div>
    </div>
    <div class="btn-mas">
        <label for="btn-mas" ><i class="fa-brands fa-whatsapp"></i></label>
    </div>
</div>

  




</template>


<style>
body {
              font-family: Arial, sans-serif;
            }
            

      *{
           margin: 0;
           padding: 0;
           box-sizing: border-box;
       }
       #btn-mas{
           display: none;
       }
       .cotenido{
           position: fixed;
           bottom: 10px;
           left: 20px;
             z-index:99;
       }
       .redes {
         display: flex;
         flex-direction: column;
         width: 250px;
         opacity: 0;
         transition: all 500ms ease;
         visibility: hidden;
         box-shadow: 0px 1px 10px rgba(0,0,0,0.4);
         border-radius: 10px;
         color: #fff;
         background: #fff;

       }
       .redes .encabezado{
         display: flex;
         flex-direction: column;
         background: #30BF42;
         color: #fff;
         padding: 15px 10px;
         border-radius: 10px 10px 0px 0px;
       }
       .redes .encabezado b{
         font-size: 20px;
         padding-bottom: 5px;
       }
       .redes .agentes  i{
         font-size: 25px;
         padding: 10px;
         margin: 5px 10px;
         color: #fff;
         background: #30BF42;
         border-radius: 100px;

       }
       .redes .agentes ul{
        list-style: none;
        padding: 15px 0;
        
       }
       .agentes{
        overflow: auto;
        max-height: 300px;

       }
       .redes .agentes li{
         color: #000;
         font-size: 18px;
         font-weight: 500;
       }
       .redes .agentes a{
         color: #000;
         text-decoration: none;
         cursor: pointer;
       }
       .redes .agentes::-webkit-scrollbar {
            -webkit-appearance: none;
        }

        .redes .agentes::-webkit-scrollbar:vertical {
            width:10px;
        }

        .redes .agentes::-webkit-scrollbar-button:increment,.redes .agentes::-webkit-scrollbar-button {
            display: none;
        } 

        .redes .agentes::-webkit-scrollbar:horizontal {
            height: 10px;
        }

        .redes .agentes::-webkit-scrollbar-thumb {
            background-color: #777;
            border-radius: 20px;
            border: 2px solid #777;
        }

        .redes .agentes::-webkit-scrollbar-track {
            border-radius: 10px;  
        }
               
       .btn-mas label{
           display: block;
           text-decoration: none;
           font-size: 30px;
           color: #fff !important;
           width: 55px;
           height: 55px;
           line-height:50px;
           text-align: center;
           padding: 5px;
           border-radius: 50%;
           box-shadow: 0px 1px 10px rgba(0,0,0,0.4);
           transition: all 500ms ease;
         }

       
       #btn-mas:checked~ .redes {
           margin-bottom: 5px;
           opacity: 1;
           visibility: visible;
       }
       .btn-mas label{
           cursor: pointer;
           background: #30BF42;
           font-size: 30px;

       }







</style>

<script>




</script>