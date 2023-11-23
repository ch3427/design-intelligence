<template>
  <div class="landing-page">
    <header>
      <h1>Learn Lean Product Management</h1>
      <p>Unlock the secrets of efficient product development with lean principles.</p>
    </header>

    <section class="introduction">
      <h2>Introduction</h2>
      <p>
        Welcome to our comprehensive Lean Product Management course! Whether you're a seasoned product manager or just
        starting, this course will equip you with the skills and knowledge to streamline your product development
        process.
      </p>
      <img src="https://via.placeholder.com/800x400" alt="Lean Product Management" />
    </section>

    <section class="key-concepts">
      <h2>Key Concepts</h2>
      <ul>
        <li>Build-Measure-Learn Cycle</li>
        <li>Minimum Viable Product (MVP)</li>
        <li>Continuous Improvement</li>
        <li>Customer Development</li>
        <li>Lean Canvas</li>
        <li>Kanban Methodology</li>
        <li>Business Model Canvas</li>
      </ul>
      <img src="https://via.placeholder.com/800x400" alt="Key Concepts" />
    </section>

    <section class="resources">
      <h2>Resources</h2>
      <p>Explore these resources to deepen your understanding of Lean Product Management:</p>
      <ul>
        <li><a href="https://www.lean.org/" target="_blank">Lean Enterprise Institute</a></li>
        <li><a href="https://leanstack.com/" target="_blank">Lean Stack</a></li>
        <li><a
            href="https://www.amazon.com/Lean-Startup-Entrepreneurs-Continuous-Innovation/dp/0307887898"
            target="_blank">The Lean Startup by Eric Ries</a></li>
        <li><a href="https://www.youtube.com/watch?v=2tbc92bPz7s" target="_blank">Introduction to Lean Product
            Management</a></li>
        <li><a href="https://en.wikipedia.org/wiki/Business_Model_Canvas" target="_blank">Business Model Canvas</a></li>
      </ul>
      <img src="https://via.placeholder.com/800x400" alt="Lean Product Management Resources" />
    </section>

    <section class="business-model-canvas">
      <h2>Business Model Canvas</h2>
      <p>Explore and interact with the Business Model Canvas below:</p>
      <!-- Embed an interactive Business Model Canvas here (replace with your preferred embed code) -->
      <iframe src="https://www.businessmodelcanvas.org/" width="800" height="600" frameborder="0" allowfullscreen></iframe>
    </section>

    <section class="chatbot">
      <h2>Live Chat Support</h2>
      <p>Have questions? Chat with our expert now!</p>
      <!-- Placeholder for a chatbot (replace with your actual chatbot implementation) -->
      <div class="chatbot-container">
        <p>This is where the chatbot will be embedded.</p>
      </div>
    </section>

    <section class="cta">
      <h2>Ready to Get Started?</h2>
      <p>Enroll now and take the first step towards becoming a Lean Product Management expert!</p>
      <button @click="enrollNow">Enroll Now</button>
    </section>

    <footer>
      <p>&copy; 2023 Lean Product Management Institute. All rights reserved.</p>
    </footer>
  </div>
</template>

<script>
export default {
  methods: {
    enrollNow() {
      // Implement your enrollment logic here
      alert('Enrollment logic goes here!');
    }
  }
};
</script>

<style scoped>
/* Your styles go here */

/* Example style for images */
img {
  max-width: 100%;
  height: auto;
  margin-top: 20px;
}

/* Additional styling for sections */
.introduction,
.key-concepts,
.resources,
.business-model-canvas,
.chatbot,
.cta {
  margin-bottom: 40px;
}

/* Example style for the chatbot container */
.chatbot-container {
  border: 1px solid #ccc;
  padding: 10px;
  max-width: 600px;
  margin: 20px auto;
}
</style>
