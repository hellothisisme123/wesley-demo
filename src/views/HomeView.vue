<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <main>
    <h1 class="title">Hello, this is for web development tools</h1>
    <h2>There's going to be all sorts of web development tools here like, color pickers, font pickers, file type to file type converters, and many many more</h2>
    <p>I don't intend on working on this very often, but whenever I find inspiration I'll make an update</p>
  </main>
</template>

<style>
  main {
    padding-top: 5%;
    display: flex;
    flex-direction: column;
  }

  .title {
    color: var(--color-text);
    text-align: center;
  }
</style>