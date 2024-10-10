<template>
  <div id="app">
    <AppHeader />
    <section class="artist-container"> 
      <h1 class="artist-name">Vincent Van Gogh</h1>
    </section>
    <main>
      <section class="button-container">
        <router-link to="/Paintings" class="button" aria-label="Navigate to Paintings">
          <img src="./assets/loyola2.png" alt="Paintings" />
          <span>Paintings</span>
        </router-link>
        <router-link to="/Drawings" class="button">
          <img src="./assets/loyola2.png" alt="Drawings" aria-label="Navigate to Drawings"/>
          <span>Drawings</span>
        </router-link>
        <router-link to="/Sculptures" class="button">
          <img src="./assets/loyola2.png" alt="Sculptures" aria-label="Navigate to Sculptures"/>
          <span>Sculptures</span>
        </router-link>
        <router-link to="/Letters" class="button">
          <img src="./assets/loyola2.png" alt="Letters" aria-label="Navigate to Letters"/>
          <span>Letters</span>
        </router-link>
      </section>
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