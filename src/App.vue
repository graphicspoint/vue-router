<script setup>
import { RouterLink, RouterView } from 'vue-router'
import Footer from './components/Footer.vue';

</script>

<template>
  <header>

    <div class="wrapper">

      <nav class="navbar navbar-expand-lg bg-light">
        <div class="container-fluid">
          <RouterLink to="/" class="navbar-brand">Navbar</RouterLink>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
            aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
              <li class="nav-item">
                <RouterLink to="/" class="nav-link active" aria-current="page" href="#">Home</RouterLink>
              </li>
              <li class="nav-item">
                <RouterLink to="/about" class="nav-link" href="#">About</RouterLink >
              </li>
              <li class="nav-item">
                <RouterLink to="/service" class="nav-link" href="#">Services</RouterLink >
              </li>
              <li class="nav-item">
                <RouterLink to="/contact" class="nav-link">Contact</RouterLink>
              </li>
            </ul>
          </div>
        </div>
      </nav>

    </div>
  </header>

  <div class="container vh-100">
    <RouterView />
  </div>
  <Footer />
</template>

<style scoped>

</style>
