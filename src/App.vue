<script setup>
import { RouterView } from 'vue-router'
import Nav from './components/Nav.vue';
</script>

<template>
  <Nav></Nav>
  <RouterView />
  <footer>&copy; Copyright 2023 Nova Mae Photography</footer>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Manrope&family=Montserrat:wght@200&family=Poppins:wght@200;300;400;500;600;700;800&display=swap');

h1,
h2,
h3,
h4 {
  font-family: 'Manrope', sans-serif;
  text-transform: uppercase;
}

p {
  font-family: 'Manrope', sans-serif;
}

footer {
  text-align: center;
  padding: 50px;
  width: 100%;
  height: 100px;
  bottom: 0;
}
</style>