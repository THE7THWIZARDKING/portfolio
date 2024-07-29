<template>
  <section class="relative h-screen overflow-hidden">
    <div
      class="absolute inset-0 w-full h-full bg-cover bg-center"
      style="
        background-image: url('https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExNWQ2YTcyM3d2N2I1MWljZHpzZTl4aWJpbDdhaDBjMHl1YmR4dTZjMiZlcD12MV9naWZzX3NlYXJjaCZjdD1n/26tn33aiTi1jkl6H6/200.webp');
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
        <a
          href="/Portfolio"
          class="bg-[#132620] hover:bg-[#B68D40] text-white py-2 px-4 rounded"
          >View My Work</a
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
