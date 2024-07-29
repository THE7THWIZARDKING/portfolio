<template>
  <section id="blog" class="py-16 bg-gray-50">
    <div class="container mx-auto px-6">
      <div class="text-center mb-12">
        <h1 class="text-4xl font-extrabold text-gray-900 mb-4">Blog</h1>
        <p class="text-lg text-gray-700 leading-relaxed">
          Welcome to my blog! Here you will find my latest thoughts, insights,
          and updates on web development and design.
        </p>
      </div>

      <!-- Blog Post List -->
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        <!-- Blog Post Item -->
        <div
          class="bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition-shadow duration-300"
        >
          <img
            src="#"
            alt="Blog Post Image"
            class="w-full h-48 object-cover rounded-t-lg mb-4"
          />
          <h2 class="text-2xl font-semibold text-gray-800 mb-2">
            Blog Post Title
          </h2>
          <p class="text-gray-700 mb-4">
            A brief excerpt from the blog post. This should give readers an idea
            of what the post is about and entice them to read more.
          </p>
          <a href="#" class="text-blue-500 hover:underline"
            >Read More</a
          >
        </div>

        <!-- Repeat Blog Post Item for each post -->
      </div>
    </div>
  </section>
</template>

<style scoped>
/* Additional styling can be added here if necessary */
</style>
