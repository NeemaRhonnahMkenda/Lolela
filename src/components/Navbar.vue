<template>
  <nav class="bg-custom-brown border-gray-200 dark:bg-custom-brown">
    <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">
      <a href="https://flowbite.com/" class="flex items-center space-x-3 rtl:space-x-reverse">
        <!--        <img src="@/assets/images/flower.svg" class="h-10" alt="LOLELA Logo"/>-->
        <span class="self-center text-3xl font-semibold whitespace-nowrap text-white dark:text-white">LOLELA</span>
      </a>
      <div class="flex items-center md:order-2 space-x-1 md:space-x-0 rtl:space-x-reverse">
        <!-- Language Dropdown -->
        <button
            type="button"
            data-dropdown-toggle="language-dropdown-menu"
            class="inline-flex items-center font-medium justify-center px-4 py-2 text-sm text-gray-900 dark:text-white rounded-lg cursor-pointer hover:bg-gray-100 dark:hover:bg-gray-700 dark:hover:text-white"
        >
          <!-- Dropdown icon -->
          <svg class="w-5 h-5 rounded-full me-3" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
               xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 3900 3900">
            <path fill="#b22234" d="M0 0h7410v3900H0z"/>
            <path d="M0 450h7410m0 600H0m0 600h7410m0 600H0m0 600h7410m0 600H0" stroke="#fff" stroke-width="300"/>
            <path fill="#3c3b6e" d="M0 0h2964v2100H0z"/>
            <g fill="#fff">
              <!-- Flag icon paths -->
            </g>
          </svg>
          English (US)
        </button>
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
            class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600"
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
                href="#"
                class="block py-2 px-3 text-white bg-blue-700 rounded md:bg-transparent md:text-blue-700 md:p-0 md:dark:text-orange-700"
                aria-current="page"
            >
              Home
            </a>
          </li>
          <li>
            <a
                href="#"
                class="block py-2 px-3 md:p-0 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
            >
              About Us
            </a>
          </li>
          <li>
            <a
                href="#"
                class="block py-2 px-3 md:p-0 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
            >
              Our Products
            </a>
          </li>
          <li>
            <a
                href="#"
                class="block py-2 px-3 md:p-0 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
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
  font-size: 25px; /* Set font size to 35px */
}
</style>

