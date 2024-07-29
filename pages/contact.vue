<template>
  <section class="min-h-screen flex items-center justify-center bg-gray-100">
    <div class="bg-white shadow-lg rounded-lg p-8 w-full max-w-lg">
      <h2 class="text-3xl font-bold text-center text-[#B68D40] mb-8">
        Contact Me
      </h2>
      <form @submit.prevent="submitForm">
        <div class="mb-4">
          <label class="block text-sm font-bold mb-2 text-[#B68D40]" for="name"
            >Name</label
          >
          <input
            type="text"
            id="name"
            v-model="form.name"
            class="shadow appearance-none border rounded w-full py-2 px-3 leading-tight focus:outline-none focus:shadow-outline"
            required
          />
        </div>
        <div class="mb-4">
          <label class="block text-sm font-bold mb-2 text-[#B68D40]" for="email"
            >Email</label
          >
          <input
            type="email"
            id="email"
            v-model="form.email"
            class="shadow appearance-none border rounded w-full py-2 px-3 leading-tight focus:outline-none focus:shadow-outline"
            required
          />
        </div>
        <div class="mb-4">
          <label
            class="block text-sm font-bold mb-2 text-[#B68D40]"
            for="subject"
            >Subject</label
          >
          <input
            type="text"
            id="subject"
            v-model="form.subject"
            class="shadow appearance-none border rounded w-full py-2 px-3 leading-tight focus:outline-none focus:shadow-outline"
            required
          />
        </div>
        <div class="mb-4">
          <label
            class="block text-sm font-bold mb-2 text-[#B68D40]"
            for="message"
            >Message</label
          >
          <textarea
            id="message"
            v-model="form.message"
            class="shadow appearance-none border rounded w-full py-2 px-3 leading-tight focus:outline-none focus:shadow-outline"
            rows="5"
            required
          ></textarea>
        </div>
        <div class="flex justify-center">
          <button
            type="submit"
            class="bg-[#132620] hover:bg-[#D6AD61] text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline"
          >
            Send Message
          </button>
        </div>
      </form>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      form: {
        name: "",
        email: "",
        subject: "",
        message: "",
      },
    };
  },
  methods: {
    submitForm() {
      // Handle form submission
      // For example, you can send the form data to your backend server or email service
      console.log("Form submitted:", this.form);
      alert("Your message has been sent!");
      // Reset the form
      this.form = {
        name: "",
        email: "",
        subject: "",
        message: "",
      };
    },
  },
};
</script>

<style scoped>
/* Add any custom styles here */
</style>
