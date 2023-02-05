<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'

const link = (to : string) => {
  console.log(to);
  
}
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
          Have you ever been having trouble picking colors for <span class="green">YOUR</span> website?
          <br>
          have you ever been stumped with a fitting second color scheme?
        </p>
        <h2>You should check out my my custom color picker</h2>
        <ul>
          <li>Multiple modes</li>
          <li>Adjustable themes</li>
          <li>Copy and save themes</li>
        </ul>
        <div class="btnWrapper">
          <RouterLink to="/colorPicker">Color Picker</RouterLink>
          <button class="colorPickerBtn" @click="link('colorPicker')">Color Picker</button>
        </div>
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

  .btnWrapper {
    display: flex;
    justify-content: center;
    margin: 0.5rem;
  }
  
  .purposes button {
    background-color: hsla(160, 100%, 37%, 1);
    transition: 0.4s;
    border-radius: 1000px;
    border: none;
    padding: 0.25rem 0.5rem;
    font-weight: 600;
    font-size: 1.25rem;
    cursor: pointer;
  }

  .purposes button:hover {
    scale: 1.1;
  }

  .purposes .title {
    margin-bottom: 1rem;
  }

  .purposes h2 {
    line-height: 1;
    padding: 0.75rem 0;
  }

  .purposes ul {
    padding: 0 1rem;
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
    padding: 0 2rem;
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