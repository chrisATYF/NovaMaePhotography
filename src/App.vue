<script setup>
import { RouterView } from 'vue-router'
import Nav from './components/Nav.vue';
</script>

<template>
  <Nav></Nav>
  <RouterView />
  <footer>&copy; Copyright 2023 Nova Mae Photography</footer>
</template>

<style scoped>
footer {
  text-align: center;
  padding: 50px;
  width: 100%;
  height: 100px;
  bottom: 0;
}
</style>