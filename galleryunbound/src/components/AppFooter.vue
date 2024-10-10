<template>
  <footer class="footer" role="contentinfo">
    <div class="footer-content">
      <h2 class="visually-hidden">Vincent Van Gogh Virtual Art Gallery</h2>
      <div class="footer-title">Follow Us</div> <!-- Visible title -->
      <nav aria-label="Social Media Links">
        <ul class="social-media">
          <li>
            <a href="https://facebook.com" target="_blank" rel="noopener noreferrer" aria-label="Facebook">
              <img class="icon" :src="fbIcon" alt="Facebook" />
            </a>
          </li>
          <li>
            <a href="https://instagram.com" target="_blank" rel="noopener noreferrer" aria-label="Instagram">
              <img class="icon" :src="igIcon" alt="Instagram" />
            </a>
          </li>
          <li>
            <a href="https://twitter.com" target="_blank" rel="noopener noreferrer" aria-label="Twitter">
              <img class="icon" :src="twitterIcon" alt="Twitter" />
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