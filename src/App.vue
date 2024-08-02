<template id="app">
  <Navbar/>
  <hero-section/>
  <about-us/>
</template>

<script>
import {defineComponent} from "vue";
import Navbar from "@/components/Navbar.vue";
import HeroSection from "@/components/HeroSection.vue";
import AboutUs from "@/components/AboutUs.vue";

export default defineComponent({
  components: {AboutUs, HeroSection, Navbar}
})
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Libre+Caslon+Display&display=swap');

#app {
  font-family: "Libre Caslon Display", serif;
  font-weight: 400;
  font-style: normal;
}
</style>
