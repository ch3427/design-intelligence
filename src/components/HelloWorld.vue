<template>
  <div class="landing-page" @mousemove="handleMouseMove">

    <!-- Chatbox -->
    <div v-if="showChatbox" class="chatbox">
      <button class="close-chatbox" @click="closeChatbox">&times;</button>
      <p>Need help?</p>
      <button @click="connectToMentor">Connect to a Mentor</button>
      <button @click="showRealLifeApplication">Show Real-Life Application</button>
      <button @click="showQuickSummary">Provide Quick Summary</button>
    </div>

    <!-- Quick Summary Modal -->
    <div v-if="showSummaryModal" class="modal">
      <div class="modal-content">
        <span class="close" @click="closeSummaryModal">&times;</span>
        <h2>Quick Summary</h2>
        <p>
          Welcome to our Lean Product Management course! This course equips you with skills to streamline product development.
          Key concepts include the Business Model Canvas, customer segmentation, and effective channels.
          Explore resources and tools to refine your business model. Connect with mentors for guidance.
        </p>
      </div>
    </div>
    
    <!-- Content -->
    <header>
      <h1>Lean Product Management</h1>
      <p>Unlock the secrets of efficient product development with lean principles.</p>
    </header>

    <section class="business-model-canvas">
      <h2>Business Model Canvas</h2>
      <p>
        The Business Model Canvas (BMC) is a powerful strategic management tool designed to swiftly and effectively define and
        communicate a business idea or concept. It serves as a one-page document that meticulously outlines the
        fundamental elements of a business or product, structuring an idea in a coherent and accessible way.
      </p>
      <img src="https://via.placeholder.com/800x400" alt="Business Model Canvas" />
      <p>
        Both external and internal factors converge around the value proposition, representing the exchange of value between
        your business and your customers or clients.
      </p>

      <h3>Purpose</h3>
      <p>Why do we use the Business Model Canvas?</p>
      <p>
        Quickly depict a comprehensive picture of the business idea. Understand the business and establish connections between
        the idea and its transformation into a viable business. Examine customer decision-making processes that influence the
        use of your systems. Provide a clear, shared understanding of the business.
      </p>

      <h3>How to Use It</h3>

      <h4>Value Proposition</h4>
      <p>
        The Value Proposition is foundational to any business or product, representing the fundamental concept of value exchange
        between your business and customers.
      </p>
      <p>
        Ask yourself: What problem am I solving? Why would someone want this problem solved? What motivates this problem?
      </p>
      <p>
        Tips: Consider Maslow’s Hierarchy of Needs to understand how your product/service addresses customer needs. If selling
        to other businesses, understand your role in fulfilling their Value Proposition.
      </p>

      <h4>Customer Segments</h4>
      <p>
        Customer Segmentation involves dividing the customer base into groups based on similarities such as age, gender,
        interests, and spending habits.
      </p>
      <p>
        Consider: Who is the problem-solving for? What characteristics define your target customers?
      </p>
      <p>
        Tip: Understand your market size to grasp the micro and macro perspectives of your market.
      </p>

      <h4>Customer Relationships</h4>
      <p>
        This aspect explores how a business interacts with its customers, whether in person, online, or through events.
      </p>
      <p>
        Examples: In-person (one-to-one), Online, Events (one-to-many)
      </p>
      <p>
        Create a User Journey Map to understand customer interactions, helping identify opportunities for automation.
      </p>

      <h4>Channels</h4>
      <p>
        Channels refer to avenues through which customers connect with your business. Consider where your customers are and how
        to reach them effectively.
      </p>
      <p>
        Ask: How do we inform our customer segment about our value proposition? Where are our customers? (social media, events, etc.)
      </p>
      <p>
        Examples of Channels: Social media, Email marketing, Networking, SEO/SEM, Content marketing
      </p>

      <h4>Key Activities</h4>
      <p>
        Key Activities are the actions your business takes to achieve the value proposition for customers.
      </p>
      <p>
        Ask: What activities does the business undertake? What resources are used? (time, expertise, distribution, etc.)
      </p>
      <p>
        Examples: Consulting, Designing, Web development
      </p>

      <h4>Key Resources</h4>
      <p>
        Identify the practical resources needed to undertake key business activities.
      </p>
      <p>
        Consider: Office space, Computers, Staff, Internet connection
      </p>
      <p>
        Examples: Office space, Computers, Hosting, People (staff)
      </p>

      <h4>Key Partners</h4>
      <p>
        List external companies or parties necessary to achieve key activities and deliver value to customers.
      </p>
      <p>
        Ask: Who else is needed to achieve the value proposition? Who are key partners to fulfill the business promise?
      </p>

      <h4>Cost Structures</h4>
      <p>
        Cost Structures encompass the monetary cost of operating the business.
      </p>
      <p>
        Consider: Costs of key activities, resources, and partnerships. Legal and insurance costs. Opportunity cost of running the business.
      </p>

      <h4>Revenue Streams</h4>
      <p>
        Revenue Streams are the ways your business converts the value proposition into financial gain.
      </p>
      <p>
        Consider: Pricing strategies aligned with solving customer problems. Various revenue models (subscription, freemium, etc.).
      </p>

      <h3>Tools to Use</h3>
      <p>
        <a href="https://canvanizer.com/" target="_blank">Canvanizer</a>, Whiteboard, Butchers Paper, Google Slides
      </p>

      <p>
        The Business Model Canvas is an invaluable tool for entrepreneurs and businesses to visualize, strategize, and innovate.
        It encourages a holistic understanding of how a business operates and generates value for its customers. Use the Canvas
        to refine your business model, identify opportunities, and create a sustainable, successful venture.
      </p>
    </section>

    <footer>
      <p>&copy; Design Intelligence Fall 2023</p>
    </footer>

  </div>
</template>

<script>
export default {
  data() {
    return {
      showChatbox: false,
      showSummaryModal: false,
      mouseMoveTimer: null,
    };
  },
  methods: {
    handleMouseMove() {
      clearTimeout(this.mouseMoveTimer);
      this.mouseMoveTimer = setTimeout(() => {
        this.showChatbox = true;
      }, 10000); // Show chatbox after 10 seconds of inactivity
    },
    closeChatbox() {
      this.showChatbox = false;
    },
    connectToMentor() {
      // Handle logic for connecting to a mentor
      console.log('Connecting to a mentor...');
    },
    showRealLifeApplication() {
      // Handle logic for showing a real-life application
      console.log('Showing real-life application...');
    },
    showQuickSummary() {
      // Show quick summary modal
      this.showSummaryModal = true;
    },
    closeSummaryModal() {
      // Close quick summary modal
      this.showSummaryModal = false;
    },
  },
};
</script>

<style scoped>
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

.close-chatbox {
  position: absolute;
  top: 5px;
  right: 10px;
  font-size: 18px;
  color: #aaa;
  cursor: pointer;
}

.chatbox:hover {
  transform: scale(1.1);
}

/* Modal Styles */
.modal {
  display: block;
  position: fixed;
  z-index: 1;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  overflow: auto;
  background-color: rgba(0, 0, 0, 0.7); /* Semi-transparent background */
}

.modal-content {
  background-color: #fefefe;
  margin: 10% auto;
  padding: 20px;
  border: 1px solid #888;
  width: 80%;
}

.close {
  color: #aaa;
  float: right;
  font-size: 28px;
  font-weight: bold;
  cursor: pointer;
}

.close:hover {
  color: black;
}
</style>
