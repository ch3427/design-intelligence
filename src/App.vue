<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div id="app">
    <HelloWorld msg="Welcome to our Art Gallery" />
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
  padding: 80px 20px; /* Increased padding for more space */
  max-width: 800px; /* Limit content width for a magazine-style layout */
  margin: 0 auto; /* Center the content */
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.1); /* Add a subtle shadow for depth */
}

/* Style the HelloWorld component for a cosmetic brand or art gallery look */
HelloWorld {
  font-size: 2em; /* Larger font size for emphasis */
  margin-top: 40px; /* Increased margin for better spacing */
  color: #c72d4d; /* Cosmetic brand color or a color associated with art */
  font-style: italic;
}
</style>
