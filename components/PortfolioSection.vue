<template>
  <section id="portfolio" class="py-12 ">
    <div class="text-center">
      <h2 class="text-4xl font-bold mb-8">Portfolio</h2>
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 -z-30">
        <div
          v-for="project in projects"
          :key="project.id"
          class="bg-white shadow-md rounded-lg overflow-hidden hover:scale-105 transform transition duration-300"
        >
          <img
            :src="project.thumbnail"
            alt="Project Thumbnail"
            class="w-full h-48 object-cover"
          />
          <div class="p-4">
            <h3 class="text-2xl font-bold mb-2">{{ project.title }}</h3>
            <p class="text-gray-600">{{ project.description }}</p>
            <a :href="project.link" class="text-blue-600 hover:underline"
              >View Project</a
            >
          </div>
        </div>
      </div>
    </div>

    <div class="-z-30">
      <div class="text-center">
        >
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 ">
          <div
            v-for="project in projects"
            :key="project.id"
            class="bg-white shadow-md rounded-lg overflow-hidden hover:scale-105 transform transition duration-300"
          >
            <img
              :src="project.thumbnail"
              alt="Project Thumbnail"
              class="w-full h-48 object-cover"
            />
            <div class="p-4">
              <h3 class="text-2xl font-bold mb-2">{{ project.title }}</h3>
              <p class="text-gray-600">{{ project.description }}</p>
              <a :href="project.link" class="text-blue-600 hover:underline"
                >View Project</a
              >
            </div>
          </div>
        </div>
      </div>

      <div class="text-center">
        >
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <div
            v-for="project in projects"
            :key="project.id"
            class="bg-white shadow-md rounded-lg overflow-hidden hover:scale-105 transform transition duration-300"
          >
            <img
              :src="project.thumbnail"
              alt="Project Thumbnail"
              class="w-full h-48 object-cover"
            />
            <div class="p-4">
              <h3 class="text-2xl font-bold mb-2">{{ project.title }}</h3>
              <p class="text-gray-600">{{ project.description }}</p>
              <a :href="project.link" class="text-blue-600 hover:underline"
                >View Project</a
              >
            </div>
          </div>
        </div>
      </div>

      <div class="text-center">
        >
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <div
            v-for="project in projects"
            :key="project.id"
            class="bg-white shadow-md rounded-lg overflow-hidden hover:scale-105 transform transition duration-300"
          >
            <img
              :src="project.thumbnail"
              alt="Project Thumbnail"
              class="w-full h-48 object-cover"
            />
            <div class="p-4">
              <h3 class="text-2xl font-bold mb-2">{{ project.title }}</h3>
              <p class="text-gray-600">{{ project.description }}</p>
              <a :href="project.link" class="text-blue-600 hover:underline"
                >View Project</a
              >
            </div>
          </div>
        </div>
      </div>

      <div class="text-center">
        >
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <div
            v-for="project in projects"
            :key="project.id"
            class="bg-white shadow-md rounded-lg overflow-hidden hover:scale-105 transform transition duration-300"
          >
            <img
              :src="project.thumbnail"
              alt="Project Thumbnail"
              class="w-full h-48 object-cover"
            />
            <div class="p-4">
              <h3 class="text-2xl font-bold mb-2">{{ project.title }}</h3>
              <p class="text-gray-600">{{ project.description }}</p>
              <a :href="project.link" class="text-blue-600 hover:underline"
                >View Project</a
              >
            </div>
          </div>
        </div>
      </div>

      <div class="text-center">
        >
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
          <div
            v-for="project in projects"
            :key="project.id"
            class="bg-white shadow-md rounded-lg overflow-hidden hover:scale-105 transform transition duration-300"
          >
            <img
              :src="project.thumbnail"
              alt="Project Thumbnail"
              class="w-full h-48 object-cover"
            />
            <div class="p-4">
              <h3 class="text-2xl font-bold mb-2">{{ project.title }}</h3>
              <p class="text-gray-600">{{ project.description }}</p>
              <a :href="project.link" class="text-blue-600 hover:underline"
                >View Project</a
              >
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
  
  <script setup>
const projects = [
  {
    id: 1,
    title: "Project One",
    description: "A short description of Project One.",
    thumbnail: "/path-to-thumbnail1.jpg",
    link: "/project-one",
  },
  {
    id: 2,
    title: "Project One",
    description: "A short description of Project One.",
    thumbnail: "/path-to-thumbnail1.jpg",
    link: "/project-one",
  },
  {
    id: 3,
    title: "Project One",
    description: "A short description of Project One.",
    thumbnail: "/path-to-thumbnail1.jpg",
    link: "/project-one",
  },
  {
    id: 4,
    title: "Project One",
    description: "A short description of Project One.",
    thumbnail: "/path-to-thumbnail1.jpg",
    link: "/project-one",
  },
  {
    id: 5,
    title: "Project One",
    description: "A short description of Project One.",
    thumbnail: "/path-to-thumbnail1.jpg",
    link: "/project-one",
  },
];
</script>
  