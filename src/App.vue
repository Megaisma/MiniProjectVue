<template>
  <div v-if="loading">
    <img src="/loader.gif" class="img-fluid center-block mx-auto d-block" alt="loader">
  </div>
  <div v-else>
    <NavbarElemen />
    <component :is="currentView" />
    <FooterElemen />
  </div>
</template>

<script>
import NavbarElemen from "./components/NavbarElemen.vue"
import HomeElemen from "./components/HomeElemen.vue"
import AboutElemen from "./components/AboutElemen.vue"
import StructureElemen from "./components/StructureElemen.vue"
import FooterElemen from "./components/FooterElemen.vue"
import ServiceElemen from "./components/ServiceElemen.vue"
import OurworksElemen from "./components/OurworksElemen.vue"
import HeadertestiElemen from "./components/HeadertestiElemen.vue"
import ContactElemen from "./components/ContactElemen.vue"

const routes = {
  '/': HomeElemen,
  '/about': AboutElemen,
  '/structure': StructureElemen,
  '/service': ServiceElemen,
  '/OurworksElemen': OurworksElemen,
  '/testiminials': HeadertestiElemen,
  '/contact': ContactElemen
}

export default {
  name: 'App',
  data() {
    return {
      loading: true,
      currentPath: window.location.hash,
      testimoni: []
    }
  },
  components: {
    NavbarElemen,
    HomeElemen,
    AboutElemen,
    StructureElemen,
    ServiceElemen,
    OurworksElemen,
    HeadertestiElemen,
    ContactElemen,
    FooterElemen
  },
  computed: {
    currentView() {
      return routes[this.currentPath.slice(1) || '/']
    }
  },
  mounted() {
    fetch("https://testimonialapi.toolcarton.com/api")
      .then((response) => response.json())
      .then((response) => {
        this.testimoni = response
        setTimeout(() => {
          this.loading = false
        }, 1000);

      }),
      window.addEventListener('hashchange', () => {
        this.currentPath = window.location.hash
      })
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

html {
  height: 100%;
}

body {
  overflow: hidden;
  overflow-y: scroll;
}

/* HIDE SCROLLBAR */

/* Hide scrollbar for Chrome, Safari and Opera */
body::-webkit-scrollbar {
  display: none;
}

/* Hide scrollbar for IE, Edge and Firefox */
body {
  -ms-overflow-style: none;
  /* IE and Edge */
  scrollbar-width: none;
  /* Firefox */
}

/* END HIDE SCROLLBAR */

/* TEXT HOVER NAVBAR */
/* Text hover */
.hover-underline-animation {
  display: inline-block;
  position: relative;
  color: white;
}

.hover-underline-animation:after {
  content: '';
  position: absolute;
  width: 100%;
  transform: scaleX(0);
  height: 2px;
  bottom: 0;
  left: 0;
  background-color: white;
  transform-origin: bottom right;
  transition: transform 0.25s ease-out;
}

.hover-underline-animation:hover:after {
  transform: scaleX(1);
  transform-origin: bottom left;
}

/* END TEXT HOVER NAVBAR */

.client {
  width: 100%;
  height: 100%;
  background-color: #6610f2;
}

.carousel-icon i {
  font-size: 5rem;
  color: rgba(255, 255, 255, 0.3);
}

.carousel-item i {
  font-size: 1.6rem;
  color: rgba(255, 255, 255, 0.3);
}

.t-card {
  padding: 1.8125rem 1.125rem;
  background-color: rgba(0, 0, 0, 0.5);
  border-radius: 1.25rem;
  color: #fff;
  height: auto;
}

.arrow-down {
  width: 0;
  height: 0;
  border-left: 1.5625rem solid transparent;
  border-right: 1.5625rem solid transparent;
  border-top: 1.25rem solid rgba(0, 0, 0, 0.5);
}
</style>
