<template>
  <div class="flex dark:bg-custom-brown">
    <div class="flex-1">
      <p class="ml-36 mt-32 text-amber-50 leading-loose underline lolela-text">LOLELA</p>
      <p class="ml-32 -mt-12 text-amber-50 tracking-widest" style="font-family: Sacramento, cursive; font-size: 35px;">skinare | cosmetics | everything in between</p>
    </div>
    <div class="" style="margin-left: 30px;">
        <img src="@/assets/images/hero-image.png" alt="Hero image" class="hero-image">
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeroSection',
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Sacramento&display=swap');

.hero-image {
  width: 700px; /* Adjust this value as needed for the maximum width */
  height: auto; /* Maintain the aspect ratio */
}

.lolela-text {
  font-size: 150px;
  text-decoration-thickness: 2px; /* Adjust this value to reduce the underline thickness */
  text-underline-offset: 30px; /* Adjust this value to change the distance between the underline and the text */
}
</style>
