<script setup>
import { ref } from 'vue'

let num = ref(0)
</script>

<template>
  <!--NAVBAR-->
  <nav class="navbar navbar-expand-lg navbar-dark bg-primary">
    <div class="container-fluid">
      <router-link class="navbar-brand" to="/">
        <img src="../public/icon.svg" alt="" height="40" class="d-inline-block align-text-center">
        PokeVite
      </router-link>

      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo03"
        aria-controls="navbarTogglerDemo03" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>


      <div class="collapse navbar-collapse" id="navbarTogglerDemo03">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <router-link class="nav-link" aria-current="page" to="/">Home</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">About</router-link>
          </li>

        </ul>
      </div>
    </div>
  </nav>

  <!-- CONTENT -->
  <div class="main">
    <router-view></router-view> <!--Onde serao renderizadas as rotas do projecto-->
  </div>

  <!--FOOTER-->
  <footer class="bg-primary text-light">
    <div>
      Design in {{ new Date().getFullYear() }}
    </div>

  </footer>
</template>

<style>
body {
  height: 100vh;
  background: rgb(48,168,239);
  background: linear-gradient(0deg, rgba(48,168,239,0.8969712885154062) 0%, rgba(66,52,21,1) 100%);

}

footer {
  position: fixed;
  bottom: 0;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 56px;
}
</style>