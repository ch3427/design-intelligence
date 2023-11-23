<template>
  <div class="landing-page">
    <header>
      <h1>Learn Lean Product Management</h1>
      <p>Unlock the secrets of efficient product development with lean principles.</p>
    </header>

    <section class="introduction">
      <h2>Introduction</h2>
      <p>
        Welcome to our Lean Product Management course! Whether you're a seasoned product manager or just starting,
        this course will equip you with the skills and knowledge to streamline your product development process.
      </p>
    </section>

    <section class="key-concepts">
      <h2>Key Concepts</h2>
      <ul>
        <li>Build-Measure-Learn Cycle</li>
        <li>Minimum Viable Product (MVP)</li>
        <li>Continuous Improvement</li>
        <li>Customer Development</li>
        <!-- Add more key concepts as needed -->
      </ul>
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
        <!-- Add more resources as needed -->
      </ul>
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
</style>
