<script setup>
</script>
<template>
    <div class="footer md:flex-col justify-center text-center md:p-5 p-3 mx-auto mt-20 bg-white text-emerald-950">
        <h1 class="text-4xl font-extrabold  p-5">Contact Us</h1>
        <div class="md:w-11/12 md:flex justify-around md:p-10">
            <div class="section1 flex-col justify-center mt-10">
                <div class="1 flex-col justify-center">
                    <p class=" text-2xl font-bold mb-5">Operating Times</p>
                    <p class=" text-lg font-medium">From 9AM - 9PM</p>
                    <p class=" text-lg font-medium">Fri - Sat</p>

                    <div class="qoute p-5 space-x-10 flex justify-center">
                        <button class="px-5 py-3 rounded-xl text-emerald-950 text-xl bg-emerald-200">Call us</button>
                        <button class="px-5 py-3 rounded-xl text-white text-xl bg-emerald-950">Email Us</button>
                    </div>
                    <!-- <img class="p-2 brightness-100 mx-auto" width="100" height="" src="/default2.svg" alt=""> -->
                </div>
            </div>
            <div class="section2 flex-col justify-center mt-10">
                <div class="1 flex-col justify-center">
                    <p class=" text-2xl font-bold mb-5">Our Phone</p>
                    <p class="py-1 text-lg font-medium">1(330)-900-FAST</p>
                    <p class="py-1 text-lg font-medium">1(331)-800-SHIP</p>
                </div>
                <img class="p-2 m-5 brightness-100 mx-auto" width="100" height="" src="/default2.svg" alt="">
            </div>
        </div>
        <div class="text text-center md:flex md:justify-end space-x-3 md:w-11/12 p-2 mt-10">
            <button class=" hover:bg-transparent hover:text-blue-900">Overview</button>
            <button class=" hover:bg-transparent hover:text-blue-900">Features</button>
            <button class=" hover:bg-transparent hover:text-blue-900">Pricing</button>
            <button class=" hover:bg-transparent hover:text-blue-900">Quotes</button>
            <button class=" hover:bg-transparent hover:text-blue-900">Help</button>
            <button class=" hover:bg-transparent hover:text-blue-900">FAQ</button>
        </div>
    </div>
    <div class="credits flex-col space-y-3 justify-center p-5">
        <img class="bg-white rounded-full mx-auto p-1 m-2 hover:bg-orange-500" width="40" height=""
            src="https://upload.wikimedia.org/wikipedia/commons/9/91/Octicons-mark-github.svg">
        <a href="https://github.com/zeiadsalhin"
            class="text-gray-100 text-center mx-auto flex justify-center hover:bg-transparent ">Credits:
            Created By Ziad</a>
    </div>
</template>
<style>
.credits {
    /* height: 60vh; */
    background: linear-gradient(0deg, rgba(0, 0, 0, 2), rgba(0, 0, 0, 0.6)), url('https://images.pexels.com/photos/6169052/pexels-photo-6169052.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500') no-repeat center fixed;
    background-size: cover;
}
</style>