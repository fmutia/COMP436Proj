<template>
  <footer class="footer" role="contentinfo">
    <div class="footer-content">
      <h2 class="visually-hidden">Follow Us</h2> <!-- Added hidden heading for accessibility -->
      <nav aria-label="Social Media Links"> <!-- Added navigation role for better semantics -->
        <ul class="social-media">
          <li>
            <a href="https://facebook.com" target="_blank" rel="noopener noreferrer" aria-label="Facebook">
              <img class="icon" :src="fbIcon" alt="Facebook" />
            </a>
          </li>
          <li>
            <a href="https://twitter.com" target="_blank" rel="noopener noreferrer" aria-label="Twitter">
              <img class="icon" :src="twitterIcon" alt="Twitter" />
            </a>
          </li>
          <li>
            <a href="https://instagram.com" target="_blank" rel="noopener noreferrer" aria-label="Instagram">
              <img class="icon" :src="igIcon" alt="Instagram" />
            </a>
          </li>
        </ul>
      </nav>
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
  list-style: none; /* Remove default list styling */
  padding: 0; /* Remove padding */
}

.social-media li {
  display: inline; /* Ensure list items display inline */
}

.icon {
  width: 24px; /* Set the size of the icons */
  height: 24px; /* Maintain aspect ratio */
}
</style>