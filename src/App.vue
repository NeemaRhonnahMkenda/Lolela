<template id="app">
  <Navbar/>
  <hero-section/>
  <about-us/>
  <our-products/>
</template>

<script>
import {defineComponent} from "vue";
import Navbar from "@/components/Navbar.vue";
import HeroSection from "@/components/HeroSection.vue";
import AboutUs from "@/components/AboutUs.vue";
import OurProducts from "@/components/OurProducts.vue";

export default defineComponent({
  components: {OurProducts, AboutUs, HeroSection, Navbar}
})
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Libre+Caslon+Display&display=swap');

#app {
  background-color: #E3CDC1;
  font-family: "Libre Caslon Display", serif;
  font-weight: 400;
  font-style: normal;
}
</style>
