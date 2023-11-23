<template>
  <div>
    <h1>{{ msg }}</h1>

    <p>
      Welcome to our e-learning platform! Explore the resources provided below.
    </p>

    <!-- Recommended IDE setup -->
    <p>
      Recommended IDE setup:
      <a href="https://code.visualstudio.com/" target="_blank">VS Code</a>
      +
      <a href="https://github.com/johnsoncodehk/volar" target="_blank">Volar</a>
    </p>

    <!-- Documentation links -->
    <p>
      <a href="https://vitejs.dev/guide/features.html" target="_blank">
        Vite Documentation
      </a>
      |
      <a href="https://v3.vuejs.org/" target="_blank">Vue 3 Documentation</a>
    </p>

    <!-- Counter button -->
    <button type="button" @click="count++">Count is: {{ count }}</button>

    <!-- Chat button -->
    <button @click="openChat">Open Chat</button>

    <!-- Chat popup -->
    <div v-if="isChatOpen" class="chat-popup">
      <!-- Replace the alert with your actual chat component -->
      <p @click="closeChat">Chat with fellow learners!</p>
    </div>

    <!-- Edit message -->
    <p>
      Edit
      <code>components/HelloWorld.vue</code> to test hot module replacement.
    </p>
  </div>
</template>

<script setup>
import { ref } from 'vue'

defineProps({
  msg: String
})

const count = ref(0)
const isChatOpen = ref(false)

const openChat = () => {
  isChatOpen.value = true
}

const closeChat = () => {
  isChatOpen.value = false
}
</script>

<style scoped>
a {
  color: #42b983;
}

/* Chat popup styles */
.chat-popup {
  position: fixed;
  bottom: 20px;
  right: 20px;
  background-color: #f1f1f1;
  border: 1px solid #ccc;
  padding: 10px;
  z-index: 1;
  cursor: pointer;
}
</style>
