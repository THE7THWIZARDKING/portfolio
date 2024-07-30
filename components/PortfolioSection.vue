<template>
  <section id="portfolio" class="py-2">
    <v-container>
      <div class="text-center">
        <h2 class="text-4xl font-bold text-[#B68D40] mb-8">Portfolio</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 -z-30">
          <div
            v-for="project in projects"
            :key="project.id"
            class="bg-white shadow-md rounded-lg overflow-hidden hover:scale-105 transform transition duration-300 items-center"
          >
            <img
              :src="project.thumbnail"
              alt="Project Thumbnail"
              class="h-40 px-24 object-cover"
            />
            <div class="p-4">
              <h3 class="text-2xl font-bold mb-2">{{ project.title }}</h3>
              <p class="text-gray-600">{{ project.description }}</p>
              <nuxt-link
                :to="project.link"
                class="text-[#B68D40] hover:underline"
                >View Project</nuxt-link
              >
            </div>
          </div>
        </div>
      </div>
    </v-container>
  </section>
</template>
  
  <script setup>
const projects = [
  {
    id: 1,
    title: "Nasst college",
    description:
      "Developed a responsive college website designed to facilitate course enrollment and streamline the admissions process. The site features an intuitive interface for students to easily browse and register for courses, apply for admissions, and access essential information. The responsive design ensures optimal performance across all devices, enhancing user experience and accessibility.",
    thumbnail: "https://dmcdharan.com/images/1678860663.png",
    link: "/portfolio",
    target: "_blank",
  },

  {
    id: 2,
    title: "Jaiswal pet Store",
    description:
      "Jaiswal Pet Store is an online e-commerce platform dedicated to providing a wide variety of pets to enthusiasts and pet lovers. This user-friendly website offers an extensive selection of pets, including dogs, cats, birds, reptiles, and small mammals. Customers can browse through detailed listings, view high-quality images, and access essential information about each pet, ensuring they make informed decisions. ",
    thumbnail:
      "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQE9UKu0wv6zmx8ICP37WhPb2dtmYn5ho_5B5s6GVJcdAtJ7FksHnXmXxm4RllZWOlEUaI&usqp=CAU",
    link: "/portfolio",
    target: "_blank",
  },
  // {
  //   id: 2,
  //   title: "Project two",
  //   description: "A short description of Project two.",
  //   thumbnail: "#",
  //   link: "/portfolio",
  // },
  // {
  //   id: 3,
  //   title: "Project three",
  //   description: "A short description of Project three.",
  //   thumbnail: "#",
  //   link: "/portfolio",
  // },
];
</script>
  