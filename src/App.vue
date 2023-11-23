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
  font-family: 'Merriweather', serif; /* Change to your preferred font for an editorial look */
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #333; /* Dark text color for a classic editorial feel */
  background-color: #f5f5f5; /* Light background color */
  padding: 60px 0; /* Adjust padding as needed */
  max-width: 800px; /* Limit content width for a magazine-style layout */
  margin: 0 auto; /* Center the content */
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.1); /* Add a subtle shadow for depth */
}

img {
  max-width: 100%;
  height: auto;
}

/* Style the HelloWorld component for an editorial touch */
HelloWorld {
  font-size: 1.5em;
  margin-top: 20px;
  color: #444;
  font-style: italic;
}
</style>
