<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <nav>
    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/about">About</RouterLink>
    <RouterLink to="/colorPicker">Color Picker</RouterLink>
  </nav>

  <RouterView />
</template>

<style scoped>

nav {
  width: 100%;
  height: 6vh;
  font-size: 12px;
  text-align: center;
  position: fixed;
  left: 0;
  top: 0;
  display: flex;
  justify-content: center;
  gap: 3rem;
  font-size: 2rem;
  z-index: 10000000;
  background: linear-gradient(var(--color-background) 50%, rgba(0, 0, 0, 0));
}

nav a {
  padding: 0 0.5rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a:hover {
  scale: 1.2;
  background-color: transparent;
}



</style>
