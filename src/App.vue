<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div id="app">
    <div class="header">
      <HelloWorld msg="Welcome to our Art Gallery" />
    </div>
  </div>
</template>

<style>
#app {
  font-family: 'Merriweather', serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: #000; /* Black background */
  color: #fff; /* White text color */
  padding: 80px 20px;
  max-width: 800px;
  margin: 0 auto;
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
}

.header {
  background-color: #fff; /* White header background */
  color: #000; /* Black text color */
  padding: 20px;
  border-radius: 10px;
}

/* Style the HelloWorld component for a cosmetic brand or art gallery look */
HelloWorld {
  font-size: 2em;
  margin-top: 20px;
  font-style: italic;
}

/* Resize the image to fit */
img {
  max-width: 100%;
  height: auto;
}
</style>
