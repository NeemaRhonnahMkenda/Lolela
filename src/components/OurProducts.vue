<template>
  <div class="mt-24 flex flex-col items-center">
    <h1 class="text-center text-[#CD5B1D] text-5xl mb-4">Our Products</h1>
    <div class="line mb-6"></div>
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-20 mx-auto" style="width: 89%">
      <!-- Loop through the first three items in the Grids array -->
      <div v-for="(item, index) in Grids.slice(0, 3)" :key="index" class="relative group">
        <img :src="item.image" alt="Product image" class="w-full h-auto object-cover"/>
        <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100
        transition-opacity duration-300 flex items-center justify-center flex-col p-4 m-auto"
             style="width: 350px; height: 350px;
          background-color: #E3CDC1;">
          <h2 class="text-white mb-2" style="font-size: 27px; font-family: Sacramento, cursive; color: #D7560F;">
            {{ item.description.heading }}</h2>
          <div class="line2 mb-6"></div>
          <p class="text-[#A46565]" style="font-size: 22px; font-family: Libre Caslon Display, sans-serif;">{{ item.description.paragraph }}</p>
        </div>
      </div>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-20 mx-auto mt-9" style="width: 89%;">
      <!-- Loop through the first three items in the Grids array -->
      <div v-for="(item, index) in Grids.slice(3, 6)" :key="index" class="relative group">
        <img :src="item.image" alt="Product image" class="w-full h-auto object-cover"/>
        <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 group-hover:opacity-100
        transition-opacity duration-300 flex items-center justify-center flex-col p-4 m-auto"
             style="width: 350px; height: 350px;
          background-color: #E3CDC1;">
          <h2 class="text-white mb-2" style="font-size: 27px; font-family: Sacramento, cursive; color: #D7560F;">
            {{ item.description.heading }}</h2>
          <div class="line2 mb-6"></div>
          <p class="text-[#A46565]" style="font-size: 22px; font-family: Libre Caslon Display, sans-serif;">{{ item.description.paragraph }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'OurProducts',
  data() {
    return {
      Grids: [
        {
          image: require('@/assets/images/product1.png'),
          description: {
            heading: 'Cutting-Edge Skincare',
            paragraph: 'Experience rejuvenation with our advanced skincare line, scientifically formulated to target specific concerns and reveal radiant skin.'
          }
        },
        {
          image: require('@/assets/images/product2.png'),
          description: {
            heading: 'Modern Make-up',
            paragraph: 'Elevate your look with our innovative makeup range, offering long-lasting formulas and vibrant colours for effortless beauty.'
          }
        },
        {
          image: require('@/assets/images/product3.png'),
          description: {
            heading: 'Luxury Beauty',
            paragraph: 'Indulge in opulence with our luxurious beauty products, crafted with the finest ingredients for a decadent experience.'
          }
        },
        {
          image: require('@/assets/images/product4.png'),
          description: {
            heading: 'Personalised Solutions',
            paragraph: 'Say hello to tailored skincare routines with our specialised products, designed to address individual needs effectively.'
          }
        },
        {
          image: require('@/assets/images/product5.png'),
          description: {
            heading: 'Professional Grade \n' +
                'Make-up',
            paragraph: 'Unleash your creativity with our professional makeup line trusted by artists worldwide, delivering flawless results with every application.'
          }
        },
        {
          image: require('@/assets/images/image2.png'),
          description: {
            heading: 'Tech-Driven Beauty',
            paragraph: 'Embrace the future of beauty with our advanced products, harnessing cutting-edge technology for visible, transformative results.'
          }
        },
      ],
    }
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Sacramento&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Libre+Caslon+Display&display=swap');

.line {
  width: 200px; /* Adjust the width as needed */
  height: 3px; /* Adjust the height as needed */
  background-color: #CD5B1D; /* Match the color of the text */
}

.line2 {
  width: 150px; /* Adjust the width as needed */
  height: 1px; /* Adjust the height as needed */
  background-color: #DCADAD; /* Match the color of the text */
}

.relative {
  position: relative;
}

.group:hover .group-hover\:opacity-100 {
  opacity: 1;
}

.absolute {
  position: absolute;
}

.bg-black {
  background-color: #000;
}

.bg-opacity-50 {
  background-color: rgba(0, 0, 0, 0.5);
}

.transition-opacity {
  transition: opacity 0.3s;
}

.text-white {
  color: #fff;
}

.flex {
  display: flex;
}

.items-center {
  align-items: center;
}

.justify-center {
  justify-content: center;
}

.p-4 {
  padding: 1rem; /* Adjust as needed */
}

.object-cover {
  object-fit: cover;
}
</style>

