<template>
  <div class="mt-24 flex flex-col items-center">
    <h1 class="text-center text-[#CD5B1D] text-5xl mb-4">Contact Us</h1>
    <div class="line mb-6"></div>

    <div class="square p-8 grid grid-cols-2 gap-4">
      <!-- left Column (Form) -->
      <div class="flex justify-center items-center">
        <form class="w-full max-w-lg form">
          <div class="flex flex-wrap -mx-3 mb-6">
            <div class="w-full md:w-1/2 px-3 mb-6 md:mb-0">
<!--              <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="first-name">-->
<!--                First Name-->
<!--              </label>-->
              <input
                  class="shadow appearance-none block w-full bg-white bg-opacity-70 text-gray-700 border border-gray-200 rounded-lg py-3 px-4 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
                  id="first-name" type="text" placeholder="First Name">
            </div>
            <div class="w-full md:w-1/2 px-3">
<!--              <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="last-name">-->
<!--                Last Name-->
<!--              </label>-->
              <input
                  class="shadow appearance-none block w-full bg-white bg-opacity-70 text-gray-700 border border-gray-200 rounded-lg py-3 px-4 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
                  id="last-name" type="text" placeholder="Last Name">
            </div>
          </div>
          <div class="flex flex-wrap -mx-3 mb-8">
            <div class="w-full px-3">
<!--              <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="email">-->
<!--                Email-->
<!--              </label>-->
              <input
                  class="shadow appearance-none block w-full bg-white bg-opacity-70 text-gray-700 border border-gray-200 rounded-lg py-3 px-4 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
                  id="email" type="email" placeholder="Email">
            </div>
          </div>
          <div class="flex flex-wrap -mx-3 mb-8">
            <div class="w-full px-3">
<!--              <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="message">-->
<!--                Message-->
<!--              </label>-->
              <textarea
                  class="shadow appearance-none block w-full bg-white bg-opacity-70 text-gray-700 border border-gray-200 rounded-xl
                  py-3 px-4 leading-tight focus:outline-none focus:bg-white focus:border-gray-500 h-48 resize-none"
                  id="message" placeholder="Message..."></textarea>
            </div>
          </div>
          <div class="flex flex-wrap -mx-3 mb-4">
            <div class="w-full px-3">
              <button
                  class="bg-[#C16937] text-white py-2 px-12 rounded hover:bg-[#B44C1A] focus:outline-none focus:bg-[#B44C1A] shadow"
                  style="border-radius: 25px;">
                SUBMIT
              </button>
            </div>
          </div>
        </form>
      </div>

      <!-- right Column (Empty) -->
      <div class="info">
        <div class="mt-6 flex flex-col m-auto items-center justify-center border rounded border-[#D6D6D6] p-6" style="border-style: solid; margin-left: 20px; margin-right: 20px; border-radius: 25px;">
          <h1 style="font-size: 25px; letter-spacing: 3px;">Company Email/Phone</h1>
          <div style="width: 400px; height: 1px; background-color: rgba(99,99,99,0.2); margin-top: 10px; margin-bottom: 8px"></div>
          <p class="mt-2" style="font-weight: bold; font-size: 20px; letter-spacing: 3px;">lolela-zm@gmail.com</p>
          <p class="mt-2" style="font-weight: bold; font-size: 20px; letter-spacing: 3px;">+260777037074 </p>
        </div>
        <div class="mt-10 flex flex-col m-auto items-center justify-center border rounded border-[#D6D6D6] p-6" style="border-style: solid; margin-left: 20px; margin-right: 20px; border-radius: 25px;">
          <h1 style="font-size: 25px; letter-spacing: 3px;">Opening Hours</h1>
          <div style="width: 400px; height: 1px; background-color: rgba(99,99,99,0.2); margin-top: 10px; margin-bottom: 8px;"></div>
          <p class="mt-2" style="font-weight: bold; font-size: 20px; letter-spacing: 3px;"><span style="color: #DCB900;">8AM - 6PM</span> Weekdays</p>
          <p class="mt-2" style="font-weight: bold; font-size: 20px; letter-spacing: 3px;"><span style="color: #DCB900;">9AM - 4PM</span> Weekends</p>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: 'ContactUs',
  data() {
    return {}
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Sacramento&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Libre+Caslon+Display&display=swap');

.line {
  width: 190px; /* Adjust the width as needed */
  height: 3px; /* Adjust the height as needed */
  background-color: #BC6A6A; /* Match the color of the text */
}

.square {
  width: 1350px;
  height: 500px;
  background-color: rgba(205, 91, 29, 0.2);
  border-radius: 25px;
}

.form {
  font-family: "Libre Caslon Display", sans-serif;
  font-size: 20px;
}

.info {
  width: 600px;
  height: 450px;
  background-color: rgba(255, 255, 255, 0.7);
  margin-left: 30px;
  border-radius: 20px;
}
</style>

