<script setup>
import { RouterView } from 'vue-router'
import Nav from './components/Nav.vue';
</script>

<template>
  <Nav></Nav>
  <RouterView />
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Manrope&family=Montserrat:wght@200&family=Poppins:wght@200;300;400;500;600;700;800&display=swap');

h1,
h2,
h3,
h4,
h5 {
  font-family: 'Manrope', sans-serif;
  text-transform: uppercase;
  letter-spacing: 3px;
}

p {
  font-family: 'Manrope', sans-serif;
  letter-spacing: 2px;
}
</style>