<template>

<nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item">
          <router-link to="/" class="nav-link active" aria-current="page">Inicio</router-link>
        </li>
        <li class="nav-item">
          <router-link to="/serviciopsicologo" class="nav-link" >Servicios</router-link>
        </li>
        <li class="nav-item">
          <router-link to="/contactopsicologo" class="nav-link">Contacto</router-link>
        </li>
        <li class="nav-item">
          <router-link to="/sebastianvillagarcia" class="nav-link">¿Quien soy?</router-link>
        </li>
      </ul>
    </div>
  </div>
</nav>
</template>

<script setup>

</script>

<style>


/* Barra de navegación celeste con letras grises */
.navbar {
  background-color: #00bfff; /* Color celeste */
}

.navbar .navbar-nav .nav-link {
  color: gray; /* Letras grises */
}

</style>