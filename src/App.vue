<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div id="app">
    <header>
      <img alt="Cosmetic Brand Logo" src="./assets/logo.png" />
      <h1>Your Beauty, Redefined</h1>
      <p>Discover the Art of Radiance</p>
    </header>

    <section class="hero">
      <img alt="Cosmetic Products" src="./assets/hero-image.jpg" />
    </section>

    <section class="introduction">
      <h2>Welcome to Our Beauty Haven</h2>
      <p>
        Indulge in the world of beauty and transform your look with our exquisite range of cosmetic products. Experience
        the perfect blend of quality and style.
      </p>
    </section>

    <section class="key-concepts">
      <h2>Discover Our Collection</h2>
      <p>Explore a curated collection designed to enhance your natural beauty:</p>
      <ul>
        <li>Luxurious Skincare</li>
        <li>Elegant Makeup Essentials</li>
        <li>Sophisticated Fragrances</li>
      </ul>
    </section>

    <section class="testimonial">
      <h2>What Our Customers Say</h2>
      <p>"Absolutely in love with the quality of these products. My go-to for a flawless finish!"</p>
      <p>- Happy Customer</p>
    </section>

    <section class="cta">
      <h2>Experience True Beauty</h2>
      <p>Shop our exclusive collection and redefine your beauty routine.</p>
      <button @click="exploreCollection">Explore Now</button>
    </section>

    <footer>
      <p>&copy; 2023 Your Beauty, Redefined. All Rights Reserved.</p>
    </footer>
  </div>
</template>

<style>
#app {
  font-family: 'Montserrat', sans-serif; /* Change to your preferred font for a cosmetic brand look */
  color: #333; /* Dark text color for readability */
  text-align: center;
}

header {
  background-color: #fff; /* White background for the header */
  padding: 20px;
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.1); /* Add a subtle shadow for depth */
}

header img {
  max-width: 100px; /* Adjust logo size as needed */
}

header h1 {
  margin-bottom: 10px;
  color: #e44d26; /* Brand color for emphasis */
}

.hero img {
  width: 100%; /* Make the hero image fill the width of its container */
}

.introduction {
  background-color: #f9f9f9; /* Light gray background for the introduction section */
  padding: 40px 20px;
}

.key-concepts ul {
  list-style-type: none; /* Remove bullet points for a cleaner look */
  padding: 0;
}

.key-concepts li {
  margin-bottom: 10px;
}

.testimonial {
  background-color: #fafafa; /* Very light gray background for the testimonial section */
  padding: 20px;
}

.cta {
  background-color: #e44d26; /* Brand color for the call-to-action section */
  color: #fff; /* White text for contrast */
  padding: 40px 20px;
}

button {
  background-color: #333; /* Dark button color for contrast */
  color: #fff; /* White text for the button */
  padding: 10px 20px;
  border: none;
  cursor: pointer;
  font-size: 1em;
  transition: background-color 0.3s ease-in-out;
}

button:hover {
  background-color: #555; /* Darker color on hover for a subtle effect */
}

footer {
  background-color: #333; /* Dark background for the footer */
  color: #fff; /* White text for the footer */
  padding: 10px 0;
}
</style>
