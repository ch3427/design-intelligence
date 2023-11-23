<template>
  <div class="landing-page" @mousemove="handleMouseMove">

    <!-- Chatbox -->
    <div v-if="showChatbox" class="chatbox" @click="toggleChatbox">
      <!-- Placeholder for your chatbox content -->
      <p>This is where the chatbox content will be.</p>
    </div>
    
    <!-- ... (existing content) -->
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
        <!-- ... (previous key concepts) -->
        <li>Business Model Canvas</li>
      </ul>
      <img src="https://via.placeholder.com/800x400" alt="Key Concepts" />
    </section>

    <section class="resources">
      <h2>Resources</h2>
      <p>Explore these resources to deepen your understanding of Lean Product Management:</p>
      <ul>
        <!-- ... (previous resources) -->
        <li><a href="https://en.wikipedia.org/wiki/Business_Model_Canvas" target="_blank">Business Model Canvas</a></li>
      </ul>
      <img src="https://via.placeholder.com/800x400" alt="Lean Product Management Resources" />
    </section>

    <section class="business-model-canvas">
      <h2>Business Model Canvas</h2>
      <p>
        The Business Model Canvas (BMC) is a powerful strategic management tool designed to swiftly and effectively define and
        communicate a business idea or concept. It serves as a one-page document that meticulously outlines the
        fundamental elements of a business or product, structuring an idea in a coherent and accessible way.
      </p>
      <p>
        An exemplary Business Model Canvas consists of two main sections. The right side focuses on the external perspective,
        specifically the customer, while the left side concentrates on internal aspects related to the business.
      </p>
      <img src="https://via.placeholder.com/800x400" alt="Business Model Canvas" />
      <p>
        Both external and internal factors converge around the value proposition, representing the exchange of value between
        your business and your customers or clients.
      </p>

      <h3>Purpose</h3>
      <p>Why do we use the Business Model Canvas?</p>
      <ul>
        <li>Quickly depict a comprehensive picture of the business idea.</li>
        <li>Understand the business and establish connections between the idea and its transformation into a viable business.</li>
        <li>Examine customer decision-making processes that influence the use of your systems.</li>
        <li>Provide a clear, shared understanding of the business.</li>
      </ul>

      <h3>How to Use It</h3>

      <h4>Value Proposition</h4>
      <p>
        The Value Proposition is foundational to any business or product, representing the fundamental concept of value exchange
        between your business and customers.
      </p>
      <p>Ask yourself:</p>
      <ul>
        <li>What problem am I solving?</li>
        <li>Why would someone want this problem solved?</li>
        <li>What motivates this problem?</li>
      </ul>
      <p>Tips:</p>
      <ul>
        <li>Consider Maslow’s Hierarchy of Needs to understand how your product/service addresses customer needs.</li>
        <li>If selling to other businesses, understand your role in fulfilling their Value Proposition.</li>
      </ul>

      <h4>Customer Segments</h4>
      <p>
        Customer Segmentation involves dividing the customer base into groups based on similarities such as age, gender, interests,
        and spending habits.
      </p>
      <p>Consider:</p>
      <ul>
        <li>Who is the problem-solving for?</li>
        <li>What characteristics define your target customers?</li>
      </ul>
      <p>Tip: Understand your market size to grasp the micro and macro perspectives of your market.</p>

      <h4>Customer Relationships</h4>
      <p>
        This aspect explores how a business interacts with its customers, whether in person, online, or through events.
      </p>
      <p>Examples:</p>
      <ul>
        <li>In-person (one-to-one)</li>
        <li>Online</li>
        <li>Events (one-to-many)</li>
      </ul>
      <p>Create a User Journey Map to understand customer interactions, helping identify opportunities for automation.</p>

      <h4>Channels</h4>
      <p>Channels refer to avenues through which customers connect with your business. Consider where your customers are and how to reach them effectively.</p>
      <p>Ask:</p>
      <ul>
        <li>How do we inform our customer segment about our value proposition?</li>
        <li>Where are our customers? (social media, events, etc.)</li>
      </ul>
      <p>Examples of Channels:</p>
      <ul>
        <li>Social media</li>
        <li>Email marketing</li>
        <li>Networking</li>
        <li>SEO/SEM</li>
        <li>Content marketing</li>
      </ul>

      <h4>Key Activities</h4>
      <p>Key Activities are the actions your business takes to achieve the value proposition for customers.</p>
      <p>Ask:</p>
      <ul>
        <li>What activities does the business undertake?</li>
        <li>What resources are used? (time, expertise, distribution, etc.)</li>
      </ul>
      <p>Examples:</p>
      <ul>
        <li>Consulting</li>
        <li>Designing</li>
        <li>Web development</li>
      </ul>

      <h4>Key Resources</h4>
      <p>Identify the practical resources needed to undertake key business activities.</p>
      <p>Consider:</p>
      <ul>
        <li>Office space</li>
        <li>Computers</li>
        <li>Staff</li>
        <li>Internet connection</li>
      </ul>
      <p>Examples:</p>
      <ul>
        <li>Office space</li>
        <li>Computers</li>
        <li>Hosting</li>
        <li>People (staff)</li>
      </ul>

      <h4>Key Partners</h4>
      <p>List external companies or parties necessary to achieve key activities and deliver value to customers.</p>
      <p>Ask:</p>
      <ul>
        <li>Who else is needed to achieve the value proposition?</li>
        <li>Who are key partners to fulfill the business promise?</li>
      </ul>

      <h4>Cost Structures</h4>
      <p>Cost Structures encompass the monetary cost of operating the business.</p>
      <p>Consider:</p>
      <ul>
        <li>Costs of key activities, resources, and partnerships.</li>
        <li>Legal and insurance costs.</li>
        <li>Opportunity cost of running the business.</li>
      </ul>

      <h4>Revenue Streams</h4>
      <p>Revenue Streams are the ways your business converts the value proposition into financial gain.</p>
      <p>Consider:</p>
      <ul>
        <li>Pricing strategies aligned with solving customer problems.</li>
        <li>Various revenue models (subscription, freemium, etc.).</li>
      </ul>

      <h3>Tools to Use</h3>
      <ul>
        <li><a href="https://canvanizer.com/" target="_blank">Canvanizer</a></li>
        <li>Whiteboard</li>
        <li>Butchers Paper</li>
        <li>Google Slides</li>
      </ul>

      <p>
        The Business Model Canvas is an invaluable tool for entrepreneurs and businesses to visualize, strategize, and innovate.
        It encourages a holistic understanding of how a business operates and generates value for its customers. Use the Canvas
        to refine your business model, identify opportunities, and create a sustainable, successful venture.
      </p>
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
  data() {
    return {
      showChatbox: false,
      mouseMoveTimer: null,
    };
  },
  methods: {
    handleMouseMove() {
      clearTimeout(this.mouseMoveTimer);
      this.mouseMoveTimer = setTimeout(() => {
        this.showChatbox = true;
      }, 2000);
    },
    toggleChatbox() {
      this.showChatbox = !this.showChatbox;
    },
  },
};
</script>

<style scoped>
/* ... (existing styles) */

/* Chatbox Styles */
.chatbox {
  position: fixed;
  bottom: 20px;
  right: 20px;
  background-color: #1a1a1a; /* Dark background color */
  color: #fff; /* Text color */
  border: 1px solid #333;
  padding: 10px;
  transition: transform 0.3s ease-in-out;
  cursor: pointer;
}

.chatbox:hover {
  transform: scale(1.1);
}

/* Styling for bullet points */
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}

ul li {
  margin-bottom: 10px;
  position: relative;
}

ul li:before {
  content: "•";
  color: #007bff; /* Bullet point color */
  font-size: 18px;
  position: absolute;
  left: -20px;
}
</style>
