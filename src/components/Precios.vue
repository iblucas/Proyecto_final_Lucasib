<template>


<section id="pricing">

<div class="row">
      <div class="pricing-column col-lg-4 col-md-6">
        <div class="card">
          <div class="card-header">
            <h3>FREE</h3>
          </div>
          <div class="card-body">
            <h2>Gratis</h2>
            <p>45 min</p>
            <p>1 sesion</p>
            <button class="btn btn-lg btn-block btn-dark" type="button">PIDE CITA</button>
          </div>
        </div>
      </div>
    
      <div class="pricing-column col-lg-4 col-md-6">
        <div class="card">
          <div class="card-header">
            <h3>PRESENCIAL</h3>
          </div>
          <div class="card-body">
            <h2>70€</h2>
            <p>45 min</p>
            <p> 1 sesión por semana</p>
            <button class="btn btn-lg btn-block btn-dark" type="button">PIDE CITA</button>
          </div>
        </div>
      </div>
    
      <div class="pricing-column col-lg-4">
        <div class="card">
          <div class="card-header">
            <h3>MENSUAL</h3>
          </div>
          <div class="card-body">
            <h2>250€ </h2>
            <p>Presencial - Online</p>
            <p> 4 sesiones mensuales</p>
            <button class="btn btn-lg btn-block btn-dark" type="button">PIDE CITA</button>
          </div>
        </div>
      </div>

    </div>
    </section>



</template>


<style>


html, body {
  height: 100%;
}

.row {
  height: 100%;
  align-items: center;
}

#pricing {
  height: 100%;
  padding: 100px;
  text-align: center;
}

.card {
  border: 1px solid rgb(27, 137, 211);
}

.card-header {
  color: white;
  background-color: rgb(27, 137, 211);
}

.pricing-column {
  padding: 3% 2%;
}

.btn-dark {
  background-color: rgb(27, 137, 211);
}

.btn-dark:hover {
  background-color: #303331;
}

</style>