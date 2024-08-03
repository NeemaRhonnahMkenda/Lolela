<template id="app">
  <Navbar/>
  <hero-section/>
  <about-us/>
  <our-products/>
  <contact-us/>
  <Footer/>
</template>

<script>
import {defineComponent} from "vue";
import Navbar from "@/components/Navbar.vue";
import HeroSection from "@/components/HeroSection.vue";
import AboutUs from "@/components/AboutUs.vue";
import OurProducts from "@/components/OurProducts.vue";
import ContactUs from "@/components/ContactUs.vue";
import Footer from "@/components/Footer.vue"

export default defineComponent({
  components: {ContactUs, OurProducts, AboutUs, HeroSection, Navbar, Footer}
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
