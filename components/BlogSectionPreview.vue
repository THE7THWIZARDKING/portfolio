<template>
  <section id="blog" class="py-12 bg-gray-100">
    <v-container>
      <div class="container mx-auto text-center">
        <h2 class="text-4xl font-bold mb-8">Latest Blog Posts</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <div
            v-for="post in posts"
            :key="post.id"
            class="bg-white shadow-md rounded-lg overflow-hidden"
          >
            <img
              :src="post.image"
              alt="Blog Post Image"
              class="w-full h-48 object-cover"
            />
            <div class="p-4">
              <h3 class="text-2xl font-bold mb-2">{{ post.title }}</h3>
              <p class="text-gray-600">{{ post.excerpt }}</p>
              <a :href="post.link" class="text-blue-600 hover:underline"
                >Read More</a
              >
            </div>
          </div>
        </div>
      </div>
    </v-container>
  </section>
</template>
  
  <script setup>
const posts = [
  {
    id: 1,
    title: "Blog Post One",
    excerpt: "A short excerpt of Blog Post One.",
    image: "#",
    link: "#",
  },
  {
    id: 2,
    title: "Blog Post two",
    excerpt: "A short excerpt of Blog Post two.",
    image: "#",
    link: "#",
  },
  {
    id: 3,
    title: "Blog Post One",
    excerpt: "A short excerpt of Blog Post three.",
    image: "#",
    link: "#",
  },
];
</script>
  