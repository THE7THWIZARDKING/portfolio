<template>
  <section class="relative h-screen overflow-hidden">
    <div
      class="absolute inset-0 w-[590] bg-cover bg-center"
      style="
        background-image: url('https://media3.giphy.com/media/QDjpIL6oNCVZ4qzGs7/giphy.webp?cid=790b7611v54zsvbop3d7q2e90ygqi5elwbv1l5edbnbeh0rh&ep=v1_gifs_search&rid=giphy.webp&ct=g');
      "
    ></div>
    <div
      class="relative z-10 flex items-center justify-center h-full bg-gray-900 bg-opacity-50"
    >
      <div class="text-center text-white">
        <h1 class="text-5xl font-bold mb-4">James Shrestha - Web Developer</h1>
        <p class="text-xl mb-6">
          Crafting beautiful and functional web experiences
        </p>
        <nuxt-link
          to="/Portfolio"
          class="bg-[#132620] hover:bg-[#B68D40] text-white py-2 px-4 rounded"
          >View My Work</nuxt-link
        >
      </div>
    </div>
  </section>
</template>

<style scoped>
/* Ensure the background image is displayed correctly */
.bg-cover {
  background-size: cover;
}
.bg-center {
  background-position: center;
}
</style>
