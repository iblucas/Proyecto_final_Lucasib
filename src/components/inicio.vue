<template>
<div id="slider">  
  <div class="slide" style="background:dodgerBlue;">
    <img src="../assets/img/amigos.jpg">
  </div>
  
  <div class="slide" style="background:coral;">
     <img src="../assets/img/pareja.jpg" >
  </div>
 
  <div class="slide" style="background:crimson;">
    <img src="../assets/img/chica.jpg" >
  </div>

  
  <!--Controlling arrows-->
  <span class="controls" onclick="prevSlide(-1)" id="left-arrow"><i class="fa fa-arrow-left" aria-hidden="true"></i>
</span>
  <span class="controls" id="right-arrow" onclick="nextSlide(1)"><i class="fa fa-arrow-right" aria-hidden="true"></i>
</span>
</div>
  <div id="dots-con">
 <span class="dot"></span><span class="dot"></span><span class="dot"></span><span class="dot"></span>
 </div>



</template>



<script>

</script>

<style>

</style>






