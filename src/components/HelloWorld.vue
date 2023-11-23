<template>
  <div class="elearning-container">
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
    <button @click="toggleChat" class="chat-button">Open Chat</button>

    <!-- Chat popup -->
    <div v-if="isChatOpen" class="chat-popup">
      <!-- Replace the input and button with your actual chat component -->
      <input v-model="chatMessage" placeholder="Type your message..." />
      <button @click="sendChatMessage">Send</button>
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
const chatMessage = ref('')

const toggleChat = () => {
  isChatOpen.value = !isChatOpen.value
}

const closeChat = () => {
  isChatOpen.value = false
}

const sendChatMessage = () => {
  // Replace this with your actual chat logic
  alert(`Sending message: ${chatMessage.value}`);
  chatMessage.value = '';
}
</script>

<style scoped>
/* Global styles */
body {
  font-family: 'Arial', sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f5f5f5;
}

/* Container styles */
.elearning-container {
  max-width: 800px;
  margin: 20px auto;
  padding: 20px;
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

/* Chat button styles */
.chat-button {
  background-color: #42b983;
  color: #fff;
  padding: 10px;
  border: none;
  cursor: pointer;
  border-radius: 4px;
}

/* Chat popup styles */
.chat-popup {
  position: fixed;
  bottom: 20px;
  right: 20px;
  background-color: #fff;
  border: 1px solid #ccc;
  padding: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

/* Chat input and button styles */
input {
  padding: 8px;
  margin-right: 8px;
  border: 1px solid #ccc;
  border-radius: 4px;
}

button {
  background-color: #42b983;
  color: #fff;
  border: none;
  padding: 8px;
  border-radius: 4px;
  cursor: pointer;
}
</style>
