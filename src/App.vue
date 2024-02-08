<script setup>
import { RouterLink, RouterView } from 'vue-router'
// import HelloWorld from './components/HelloWorld.vue'
import About from './components/About.vue'
import Features from './components/Features.vue'
import Liner from './components/Top.vue'
import Footer from './components/Footer.vue'
function m() {
  const menu = document.querySelector("#menu")
  menu.classList.toggle("active")
}
</script>

<template>
  <div class="head">
    <!--mob-->
    <nav
      class="nav bg-gray-500 bg-transparent text-gray-200 md:hidde sticky top-0 z-10 justify-between font-semibold mobile">
      <div class="flex justify-between">
        <a href="https://pactel.info" onclick=""> <img src="/default.svg" width="60" height="60"
            class="justify-between m-4" alt="logo"></a>
        <!-- <h1 style="font-weight: 800;" class="p-3 text-3xl text-gray-300">Courses</h1> -->
        <button @click="m" id="menub" class="md:hidde justify-between hover:bg-transparent">
          <div class="container dark:invert px-4">
            <div class="bar1">
              <hr class="border-2 bg-black border-black">
            </div>
            <!-- <div class="bar2">
              <hr class="border-2 bg-black border-black">
            </div> -->
            <div class="bar3">
              <hr class="border-2 bg-black border-black">
            </div>
          </div>
        </button>
      </div>
      <div class=" flex justify-center">
        <div
          class="menu notactive bg-gray-600 text-xl font-semibold transform bg-transparent text-gray-300 transition ease-in duration-500  mt-2 px-4 bg-gray-00 "
          id="menu">
          <RouterLink to="/" @click="m"><a href="#" class="block -mb-6">Home</a></RouterLink>
          <!-- <hr class="border-1 rounded border-gray-400 m- opacity-50 "> -->
          <RouterLink to="/" @click="m" id="menub" class="block p-2">Who we are</RouterLink>
          <RouterLink to="/" @click="m" id="menub" class="block p-2">Our Mission</RouterLink>
          <RouterLink to="/" @click="m" id="menub" class="block p-2">Shipping Calculator</RouterLink>
          <RouterLink to="/" @click="m" id="menub" class="block p-2">Shipping Prices</RouterLink>
          <a href="#" class="block p-4 mt-2 bg-blue-800 font-medium rounded-full">Call Us</a>
        </div>
      </div>
    </nav>

    <!---->
    <RouterView />
    <!-- <div class="bar"></div> -->
    <header class=" flex justify-center space-x-20 text-black bg-white hiddenm desktop">
      <div class="flex justify-start">
        <div class="flex justify-start mr-64"><img alt="logo" class="logo -m-1" src="/default.svg" width="100"
            height="90" />
        </div>

        <div class="my-auto">

          <nav class="text-xl font-semibold flex justify-end space-x-8">
            <RouterLink to="/" class="p-">Home</RouterLink>
            <RouterLink to="/" class="p-">Who we are</RouterLink>
            <RouterLink to="/" class="p-">Our Mission</RouterLink>
            <RouterLink to="/" class="p-">Shipping Calculator</RouterLink>
            <RouterLink to="/" class="p-">Shipping Prices</RouterLink>
            <button href="#" class="px-5 py-1 bg-blue-600 text-white font-medium rounded-full">Call Us</button>
          </nav>
        </div>
      </div>
    </header>


    <RouterView />
    <div
      class="flex-col justify-center md:text-5xl text-4xl space-y-5 p-5 md:mt-48 mt-12 mb-48 text-center text-white font-bold">
      <p>Shipping Services</p>
      <p>Worldwide</p>
    </div>
    <div class="flex-col justify-center text-5xl md:mb-20 mb-52 text-center text-white font-bold">
      <button class="hover:bg-transparent"><img alt="logo" class="logo" src="/arrow.svg" width="70"
          height="90" /></button>
    </div>
    <About />
    <Features />
    <Liner />
    <Products />
    <Top />
    <Information />
    <Footer />
  </div>
</template>

<style scoped>
.head {
  height: 100vh;
  background: linear-gradient(0deg, rgba(0, 0, 0, 3), rgba(0, 0, 0, 0.6)), url('https://www.simpleglobal.com/wp-content/uploads/2022/01/determining-shipping-costs-the-basics-banner-simple-global-blog.jpg') no-repeat center fixed;
  background-size: cover;

}

/* .bar {
  position: absolute;
  top: 0;
  width: 100%;
  backdrop-filter: blur(3px);
  -webkit-mask-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.8), transparent 100%);
} */

/* .front {
  z-index: 9999;
  top: 0;
} */

.notactive {
  text-align: center;
  z-index: 1;
  position: relative;
  overflow-y: hidden;
  width: 100%;
  height: 0vh;
  transition: ease-in 0.3s;
}

.active {
  height: 50vh;
  width: 100%;
  background: #040404;
}

.bar1,
.bar2,
.bar3 {
  width: 35px;
  height: 3px;
  background-color: #0c0c0c;
  margin: 8px 5px;
  transition: 0s;
}
</style>
