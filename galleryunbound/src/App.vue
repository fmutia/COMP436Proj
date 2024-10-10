<template>
  <div id="app">
    <AppHeader />
    <div class="artist-container">
      <h1 class="artist-name">Vincent Van Gogh</h1>
    </div>
    <main>
      <div class="button-container">
        <router-link to="/Oil Paintings" class="button">
          <img src="./assets/loyola2.png" alt="Paintings" />
          <span>Oil Paintings</span>
        </router-link>
        <router-link to="/products" class="button">
          <img src="./assets/loyola2.png" alt="Products" />
          <span>Products</span>
        </router-link>
        <router-link to="/contact" class="button">
          <img src="./assets/loyola2.png" alt="Contact" />
          <span>Contact</span>
        </router-link>
      </div>
      <!-- <img alt="Vue logo" src="./assets/logo.png">
      <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    </main>
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';
// import HelloWorld from './components/HelloWorld.vue';
import AppFooter from './components/AppFooter.vue';
import './css/style.css'; // Import your global CSS file

export default {
  name: 'App',
  components: {
    AppHeader,
    // HelloWorld,
    AppFooter,
  },
};
</script>