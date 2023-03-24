<script setup>
import { RouterLink, RouterView } from 'vue-router'
import NavbarComponent from "./components/NavbarComponent.vue";
</script>

<template>
  <header>
    <NavbarComponent />
  </header>
  <main>
    <RouterView />
  </main>
  <footer>
    <!-- footer component with all my contact stuff -->
  </footer>
</template>

<style scoped></style>
