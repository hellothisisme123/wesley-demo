<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <main>
    <h1 class="title">
        Hello
    </h1>
    
    <h2>
      There's going to be all sorts of 
      <span class="green">web development</span> 
      tools here like, 
      <span class="green">color pickers</span>, 
      <span class="green">font pickers</span>, 
      file type 
      <span class="green">converters</span>, 
      and many many more
    </h2>

    <p>I don't intend on working on this very often, but whenever I find inspiration I'll make an update</p>

    <div class="purposes">
      <div class="colorPicker">
        <div class="title">Color Picker</div>
        <p>
          Have you ever
        </p>
      </div>

      <div class="divider"></div>

      <div class="fileConverter">
        <div class="title">File Converter</div>
      </div>

      <div class="divider"></div>

      <div class="fontPicker">
        <div class="title">Font Picker</div>
      </div>
    </div>
  </main>

  
</template>

<style>
  .purposes {
    margin-top: 5vh;
    display: grid;
    grid-template-columns: 5fr 1fr 5fr 1fr 5fr;
    min-height: 50vh;
  }

  .purposes > div > .title {
    font-size: 2.5rem;
  }

  .purposes > .divider {
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
  }

  .divider::after {
    content: '';
    position: absolute;
    translate: -50% -50%;
    top: 50%;
    left: 50%;
    display: block;
    background-color: hsla(160, 100%, 37%, 1);
    height: 75%;
    width: 0.4vw;
    margin: 0 auto;
    border-radius: 1000px;
  }

  main {
    /*margin-top: 5%;*/
    display: flex;
    flex-direction: column;
  }

  .bold {
    font-weight: 700;
  }

  .title {
    color: hsla(160, 100%, 37%, 1);
    font-weight: 700;
    font-size: 3rem;
    text-align: center;
  }
</style>