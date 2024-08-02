<template>
  <div class="grid grid-cols-2">
    <div class="mt-16 ml-20">
      <img :src="currentImage" alt="Slideshow image" class="h-auto" style="width: fit-content"/>
    </div>
    <div>
      <h1 class="mt-32 ml-40 text-7xl" style="color: #CD5B1D;">Who are we?</h1>
      <div class="line ml-40"></div>
      <div class="description-lolela">
        <p>Lolela is a small sourcing business that brings you the best <span style="color: #CE4900">skincare, cosmetics & beauty products</span> from around
          the world.</p>
        <p>We source our products from reputable brands and strive to provide our clients
          with the best possible pricing.</p>
        <div class="info-box">
          <p>Sunday - Friday, 8AM to 6PM.</p>
        </div>
        <p>Online store based in Lusaka</p>
        <p>Countrywide delivery</p>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: 'AboutUs',
  data() {
    return {
      images: [
        require('@/assets/images/image1.png'),
        require('@/assets/images/image2.png'),
        require('@/assets/images/image3.png'),
        require('@/assets/images/image4.png')
      ],
      currentImageIndex: 0,
    };
  },
  computed: {
    currentImage() {
      return this.images[this.currentImageIndex];
    }
  },
  mounted() {
    this.startSlideshow();
  },
  methods: {
    startSlideshow() {
      setInterval(() => {
        this.currentImageIndex = (this.currentImageIndex + 1) % this.images.length;
      }, 3000); // Change image every 3 seconds
    }
  }
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Bellota:ital,wght@0,300;0,400;0,700;1,300;1,400;1,700&display=swap');

* {
  background-color: #E3CDC1;
}

.line {
  margin-top: 9px;
  width: 360px; /* Adjust the width as needed */
  height: 3px; /* Adjust the height as needed */
  background-color: #CD5B1D; /* Match the color of the text */
}

.description-lolela {
  font-family: "Bellota", system-ui;
  margin-right: 60px;
  margin-top: 20px;
  font-size: 25px;
  text-align: center;
}

.info-box p{
  background-color: #90543C; /* Adjust the background color as needed */
  border-radius: 30px; /* Adjust the border-radius as needed */
  display: inline-block;
  position: relative;
  color: white;
  padding-left: 12px;
  padding-right: 12px;
}
</style>
