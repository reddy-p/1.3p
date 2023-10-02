<script setup>
import { RouterView } from 'vue-router'
import NavBar from './components/NavBar.vue';
</script>

<template>
  <header>
    <NavBar></NavBar>
  </header>

  <RouterView class="main" />

</template>

<style scoped>
header { 
  width: 100%;
}
.main {
  padding: 2rem;
}
</style>
