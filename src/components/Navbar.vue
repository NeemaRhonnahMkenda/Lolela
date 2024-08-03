<template>
  <nav class="bg-custom-brown border-gray-200 dark:bg-custom-brown">
    <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">
      <a href="https://flowbite.com/" class="flex items-center space-x-3 rtl:space-x-reverse">
      </a>
      <div class="flex items-center md:order-2 space-x-2 md:space-x-0 rtl:space-x-reverse">
        <div
            class="z-50 hidden my-4 text-base list-none divide-y divide-gray-100 rounded-lg shadow dark:bg-custom-brown"
            id="language-dropdown-menu"
        >
          <!-- Language Dropdown items -->
        </div>
        <!-- Hamburger Menu Button -->
        <button
            @click="toggleMenu"
            type="button"
            class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-[#E3CDC1] focus:outline-none focus:ring-2 focus:ring-gray-200"
            aria-controls="navbar-language"
            :aria-expanded="isMenuOpen ? 'true' : 'false'"
        >
          <span class="sr-only">Open main menu</span>
          <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 17 14">
            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M1 1h15M1 7h15M1 13h15"/>
          </svg>
        </button>
      </div>
      <div
          :class="{
            'block': isMenuOpen,
            'hidden': !isMenuOpen,
            'md:block': true,
            'md:w-auto': true,
            'md:order-1': true
          }"
          class="items-center justify-between w-full bg-custom-brown dark:bg-custom-brown"
          id="navbar-language"
      >
        <ul class="flex flex-col text-lg-custom p-4 md:p-0 mt-4 border border-gray-100 rounded-lg md:space-x-16 rtl:space-x-reverse md:flex-row md:mt-0 md:border-0">
          <li>
            <a
                href="/#hero-section"
                class="block py-2 px-3 text-orange-600 rounded md:bg-transparent md:text-orange-600 md:p-0"
                aria-current="page"
            >
              Home
            </a>
          </li>
          <li>
            <a
                href="/#about-us"
                class="block py-2 px-3 md:p-0 text-white rounded hover:bg-[#E3CDC1] md:hover:bg-transparent md:hover:text-orange-600"
            >
              About Us
            </a>
          </li>
          <li>
            <a
                href="/#our-products"
                class="block py-2 px-3 md:p-0 text-white rounded hover:bg-[#E3CDC1] md:hover:bg-transparent md:hover:text-blue-700"
            >
              Our Products
            </a>
          </li>
          <li>
            <a
                href="/#contact-us"
                class="block py-2 px-3 md:p-0 text-white rounded hover:bg-[#E3CDC1] md:hover:bg-transparent md:hover:text-blue-700"
            >
              Contact Us
            </a>
          </li>
          <!-- Other menu items -->
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>

export default {
  name: 'NavBar',
  data() {
    return {
      isMenuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      console.log('Toggle Menu Clicked'); // For debugging
      this.isMenuOpen = !this.isMenuOpen;
    },
  },
}
</script>

<style scoped>
.text-lg-custom {
  font-size: 24px; /* Set font size to 35px */
}
</style>

