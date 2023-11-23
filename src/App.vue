<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Hello Vue 3 + Vite" />
  </div>
</template>

<style>
#app {
  font-family: 'Inter', sans-serif; /* Change to your preferred modern font */
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff; /* White text color for dark background */
  background-color: #2d3142; /* Dark background color with a hint of blue-gray */
  padding: 60px 0; /* Adjust padding as needed */
}

img {
  max-width: 100%;
  height: auto;
}

/* Add a pop of color to the HelloWorld component */
HelloWorld {
  color: #ffb86c; /* Pop color, adjust as needed */
}
</style>
