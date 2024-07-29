<template id="app">
  <Navbar/>
  <p>Hello there</p>
</template>

<script>
import {defineComponent} from "vue";
import Navbar from "@/components/Navbar.vue";

export default defineComponent({
  components: {Navbar}
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
