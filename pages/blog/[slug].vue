<template>
    <section id="blog-post" class="py-16 bg-gray-50">
      <div class="container mx-auto px-6">
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-8">
          <!-- Blog Post Content -->
          <div class="lg:col-span-2">
            <article class="bg-white p-6 rounded-lg shadow-md hover:shadow-xl transition-shadow duration-300">
              <img :src="blogPost.image" alt="Blog Post Image" class="w-full h-64 object-cover rounded-t-lg mb-4">
              <h1 class="text-4xl font-extrabold text-gray-900 mb-4">{{ blogPost.title }}</h1>
              <p class="text-gray-700 mb-4">
                {{ blogPost.content }}
              </p>
            </article>
          </div>
  
          <!-- Sidebar -->
          <aside class="bg-white p-6 rounded-lg shadow-md">
            <h2 class="text-2xl font-semibold text-gray-800 mb-4">Categories</h2>
            <ul class="list-disc list-inside text-gray-700 mb-8">
              <li v-for="category in categories" :key="category.id">
                <NuxtLink :to="`/blog/category/${category.slug}`" class="text-blue-500 hover:underline">{{ category.name }}</NuxtLink>
              </li>
            </ul>
  
            <h2 class="text-2xl font-semibold text-gray-800 mb-4">Recent Posts</h2>
            <ul class="list-disc list-inside text-gray-700">
              <li v-for="post in recentPosts" :key="post.id">
                <NuxtLink :to="`/blog/${post.slug}`" class="text-blue-500 hover:underline">{{ post.title }}</NuxtLink>
              </li>
            </ul>
          </aside>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    async asyncData({ params }) {
      // Fetch the blog post based on the slug from the URL
      const blogPost = await fetch(`/api/blog/${params.slug}`).then(res => res.json());
      
      // Fetch categories and recent posts
      const categories = await fetch(`/api/categories`).then(res => res.json());
      const recentPosts = await fetch(`/api/recent-posts`).then(res => res.json());
  
      return { blogPost, categories, recentPosts };
    }
  }
  </script>
  
  <style scoped>
  /* Additional styling can be added here if necessary */
  </style>
  