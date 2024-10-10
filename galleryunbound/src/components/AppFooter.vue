
<template>
  <footer class="footer">
    <div class="footer-content">
      <div class="social-media">
        <a href="https://facebook.com" target="_blank" rel="noopener noreferrer">
          <img class="icon" :src="fbIcon" alt="Facebook" />
        </a>
        <a href="https://twitter.com" target="_blank" rel="noopener noreferrer">
          <img class="icon" :src="twitterIcon" alt="Twitter" />
        </a>
        <a href="https://instagram.com" target="_blank" rel="noopener noreferrer">
          <img class="icon" :src="igIcon" alt="Instagram" />
        </a>
      </div>
    </div>
  </footer>
</template>

<script>
import fbIcon from '../assets/fb.png';
import twitterIcon from '../assets/x.webp';
import igIcon from '../assets/ig.png';

export default {
  name: 'AppFooter',
  data() {
    return {
      fbIcon,
      twitterIcon,
      igIcon,
    };
  },
};
</script>

<style scoped>
.footer {
  background-color: #333; /* Gray background */
  color: white;
  padding: 10px 0; /* Adjust padding as needed */
  width: 100%; /* Full width */
}

.footer-content {
  max-width: 1200px; /* Limit width */
  margin: 0 auto; /* Center content */
  text-align: center; /* Center align items */
}

.social-media {
  display: flex; /* Use flexbox for horizontal alignment */
  justify-content: center; /* Center icons */
  gap: 10px; /* Space between icons */
}

.icon {
  width: 24px; /* Set the size of the icons */
  height: 24px; /* Maintain aspect ratio */
}
</style>