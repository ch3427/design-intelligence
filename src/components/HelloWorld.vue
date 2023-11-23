<template>
  <div>
    <h1>{{ msg }}</h1>

    <p>
      Welcome to our e-learning platform! Watch the video tutorial below and use the resources provided.
    </p>

  

    <p>
      Recommended IDE setup:
      <a href="https://code.visualstudio.com/" target="_blank">VS Code</a>
      +
      <a href="https://github.com/johnsoncodehk/volar" target="_blank">Volar</a>
    </p>

    <p>
      <a href="https://vitejs.dev/guide/features.html" target="_blank">
        Vite Documentation
      </a>
      |
      <a href="https://v3.vuejs.org/" target="_blank">Vue 3 Documentation</a>
    </p>

    <button type="button" @click="count++">count is: {{ count }}</button>

    <!-- Popup Chat -->
    <button @click="toggleChat">Open Chat</button>
    <div v-if="isChatOpen" class="chat-popup">
      <!-- Your chat component goes here -->
      <p>Chat with fellow learners!</p>
    </div>

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

const toggleChat = () => {
  isChatOpen.value = !isChatOpen.value
}
</script>

<style scoped>
a {
  color: #42b983;
}

/* Add styles for your chat popup */
.chat-popup {
  position: fixed;
  bottom: 0;
  right: 15px;
  border: 1px solid #ccc;
  padding: 10px;
  background-color: #fff;
  max-height: 300px;
  overflow-y: auto;
}
</style>
