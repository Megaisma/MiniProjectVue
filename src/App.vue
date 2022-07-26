<template>
    <NavbarElemen />
    <HomeElemen />
    <AboutElemen />
    <StructureElemen />
    <ServiceElemen />
    <OurworksElemen />
    <TestimonialsElemen />
    <FooterElemen />
</template>

<script>
import NavbarElemen from "./components/NavbarElemen.vue"
import HomeElemen from "./components/HomeElemen.vue"
import AboutElemen from "./components/AboutElemen.vue"
import StructureElemen from "./components/StructureElemen.vue"
import FooterElemen from "./components/FooterElemen.vue"
import ServiceElemen from "./components/ServiceElemen.vue"
import OurworksElemen from "./components/OurworksElemen.vue"
import TestimonialsElemen from "./components/TestimonialsElemen.vue"

export default {
  name: 'App',
  components: {
    NavbarElemen,
    HomeElemen,
    AboutElemen,
    StructureElemen,
    ServiceElemen,
    OurworksElemen,
    TestimonialsElemen,
    FooterElemen
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
  -ms-overflow-style: none;  /* IE and Edge */
  scrollbar-width: none;  /* Firefox */
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

</style>
