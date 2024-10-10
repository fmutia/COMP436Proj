<template>
  <header :class="['header', { 'hidden': isHidden }]" role="banner">
    <div class="header-content">
      <div class="brand" role="img" aria-label="Brand Logo">
        <img src="../assets/rambler.png" alt="Brand Logo" class="brand-icon" />
        <span class="brand-name">Gallery Unbound</span>
      </div>
      <nav class="nav" aria-label="Main Navigation">
        <ul>
          <li><router-link to="/">Home</router-link></li>
          <li><router-link to="/about">About</router-link></li>
          <li><router-link to="/products">Products</router-link></li>
          <li><router-link to="/contact">Contact</router-link></li>
        <li><router-link to="/login">Login</router-link></li>

        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'AppHeader',
  data() {
    return {
      lastScrollY: 0,
      isHidden: false,
    };
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll);
  },
  beforeUnmount() {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll() {
      const currentScrollY = window.scrollY;

      // Hide header when scrolling down, show it when at the top
      this.isHidden = currentScrollY > 0 && currentScrollY > this.lastScrollY;
      this.lastScrollY = currentScrollY;
    },
  },
};
</script>