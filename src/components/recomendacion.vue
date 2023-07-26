<template>

    <div class="mainContent">

  
  
      <div class="testimonialWrapper">
        
       
        <div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="false" >
          <div class="carousel-indicators">   
          </div>
          <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"><i class="fas fa-caret-right"></i></span>
            <span class="visually-hidden">Next</span>
          </button>
        </div>
      

       
        <div class="testimonial-desktop">

          <div class="testimonial1">
              <div class="user-photo user1">                
              </div>

              <div class="user-testimonial">
                <h2>"Sesiones Online."</h2>
                <p>Decidí hacer sesiones online con Sebastián y el resultado ha sido muy gratificante, le recomiendo totalmente! </p>
                <span>Brianda</span>
              </div>            
          </div>

          <div class="testimonial2">
              <div class="user-photo user2">                
              </div>

              <div class="user-testimonial">
                <h2>"Muy profesional  y cercano"</h2>
                <p>Muy profesional y cercano a la vez. De gran ayuda, me ha dado herramientas muy buenas para abordar mi problema.</p>
                <span>Isabel</span>
              </div>
          </div>

          <div class="testimonial3">
              <div class="user-photo user3">                
              </div>

              <div class="user-testimonial">
                <h2>"Muy recomendable"</h2>
                <p>Sebastián me ha ayudado mucho. Estoy muy agradecido y contento con su trabajo. Es muy profesional. Lo recomiendo 100x100. </p>
                <span>Javi</span>
              </div>
          </div>

        </div>
        
        
      </div>
    
 


</div>




</template>


<style>


.ui-testimonials {
    background-color: #255946;
    background-image: url('');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    font-family: 'Red Hat Display', sans-serif;
}

.ui-testimonials i {
  padding-right: 10px;
}

/* video background */
#background-video {
    height: 100vh;
    width: 100vw;
    object-fit: cover;
    position: fixed;
    left: 0;
    right: 0;
    top: 0;
    bottom: 0;
    z-index: -1;
  }

.ui-testimonials .mainContent {
    padding: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
}

/* Header */
.ui-testimonials .header {
    background-color: transparent;
    text-align: center;
    width: 100%;
}

.ui-testimonials .header h1 {
    font-family: 'Dela Gothic One', cursive;
    text-shadow: 4px 4px 0px #18261E;
    background: rgb(217,177,163);
    background: linear-gradient(0deg, rgba(217,177,163,1) 36%, rgba(235,153,133,0) 36%);
    display: inline;
    font-size: 2rem;
    line-height: 1.5;
    color: #fff;
}

/* Testimonial Wrapper */
.ui-testimonials .testimonialWrapper {
    color: #fff;
    background-color: #255946;
    text-align: center;
    padding: 20px 0;
    width: 100%;
    margin-top: 40px;
    border-top: 3px solid #18261E;
    border-bottom: 3px solid #18261E;
}

.ui-testimonials .testimonialWrapper h1 {
    font-family: 'Crimson Pro', serif;
    color: #fff;
    width: 90%;
    margin: 0 auto;
}

.ui-testimonials .carousel {
    width: 95%;
    margin: 0 auto;
    max-width: 450px;
}

.ui-testimonials .carousel .carousel-inner {
    height: 420px;
    margin: 50px auto 0;
    width: 80%;
}

.ui-testimonials .user-photo {
    clip-path: circle(50% at 50% 50%);
    width: 130px;
    height: 130px;
    background-size: 100%;
    background-position: center;
    background-repeat: no-repeat;
    margin: 0 auto;
    border: 3px solid #D9B1A3;
    border-radius: 70px;
    background-color: #fff;
}

.ui-testimonials .user-photo.user1 {
    background-image: url('');
}

.ui-testimonials .user-photo.user2 {
    background-image: url('');
    background-position: center -20px;
    background-size: 150%;
}

.ui-testimonials .user-photo.user3 {
    background-image: url('');
    background-position: center -136px;
    background-size: 160%;
}

.ui-testimonials .user-testimonial {
    margin: 10px 0 0;
}

.ui-testimonials .user-testimonial h2 {
    font-family: 'Crimson Pro', serif;
    color: #D9B1A3;
    margin-bottom: 15px;
    line-height: .9;
    text-shadow: 2px 2px 0px #000;
    font-size: 1.8rem;
    background: linear-gradient(0deg, rgba(24,38,30,1) 37%, rgba(217,177,163,0) 37%);
    display: inline;
}

.ui-testimonials .user-testimonial p {
    color: #fff;
    margin-top: 20px;
}

.ui-testimonials .user-testimonial span {
    color: #D9B1A3;
    font-style: italic;
    font-size: .9rem;
}

.carousel-control-next, 
.carousel-control-prev {
    width: 5%;
}

.carousel-control-prev .carousel-control-prev-icon,
.carousel-control-next .carousel-control-next-icon {
    background-image: none;
}

.carousel-control-prev .carousel-control-prev-icon i,
.carousel-control-next .carousel-control-next-icon i {
    padding: 0;
    font-size: 1.5rem;
}

.ui-testimonials .carousel-indicators button {
    border-radius: 10px;
    background-clip: initial;
    width: 15px;
    height: 5px;
    border-top: 0px solid transparent;
}


.ui-testimonials .carousel-indicators .active {
    background-color: #D9B1A3;
}

.testimonial-desktop {
    display: none;
}

/* Footer */
.ui-testimonials .footer {
    background-color: transparent;
    width: 100%;
    text-align: center;
    padding: 20px 0;
    display: flex;
    justify-content: center;
    align-items: center;
    color: #fff;
    flex-direction: column;
}

.ui-testimonials .footer button {
    font-family: 'Crimson Pro', serif;
    background-color: #D9B1A3;
    border: none;
    color: #18261E;
    padding: 10px;
    text-shadow: none;
    font-weight: bold;
    position: relative;
    overflow: hidden;
    transition: all 0.3s linear;
}

.ui-testimonials .footer button:active,
.ui-testimonials .footer button:focus {
    position: relative;
    box-shadow: 0px 2px 0px #3B594B;
    padding-left: 30px;
}

.ui-testimonials .footer button i {
    position: absolute;
    left: -30px;
    top: 15px;
    transition: all 0.3s linear;
}

.ui-testimonials .footer button:active i,
.ui-testimonials .footer button:focus i {
    left: 6px;
}

.ui-testimonials .footer .footer-socmed {
    text-align: center;
    margin-top: 10px;
}

.ui-testimonials .footer .footer-socmed > i:nth-child(4) {
    padding-right: 0;
}

.ui-testimonials .footer .footer-socmed p {
    margin-bottom: 0;
}


@media screen and (min-width: 480px) {
    .ui-testimonials .footer {
        flex-direction: row;
        justify-content: space-evenly;
    }

    .ui-testimonials .footer .footer-socmed {
        text-align: right;
        margin-top: 0;
    }
}

@media screen and (min-width: 991px) {
    .ui-testimonials .header h1 {
        font-size: 3.4rem;
    }

    .ui-testimonials .carousel {
        display: none;
    }

    .testimonial-desktop {
        display: flex;
        align-items: flex-start;
        justify-content: center;
        margin: 60px auto 30px;
        width: 100%;
        max-width: 900px;
    }

    .testimonial-desktop > div {
        width: 33.3%;
        padding: 0 20px;
        transition: all 0.3s linear; 
    }

    .testimonial-desktop > div:hover {
        scale: 1.2;
        margin-top: -10px; 
    }

    .testimonial-desktop:has(div:hover) > div:not(:hover) {
        filter: blur(10px);
        opacity: 0.5;
    }

    .ui-testimonials .footer {
        max-width: 900px;
        justify-content: space-between;
    }
}

</style>



<script>




</script>