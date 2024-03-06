<template>
  <section class="p-6">
    <div class="container mx-auto mt-40">
      <div class="title">
        <h3 class="text-center md:text-left font-bold text-gray-700 mb-5">
          Check out my latest articles
        </h3>
        <h1
          class="max-w-lg text-4xl font-bold text-center text-gray-700 md:text-5xl md:text-left"
        >
          My Blog Posts
        </h1>
      </div>

      <div class="mt-20 grid gap-4" v-if="blogs.length">
        <accordions v-for="(blog, index) in blogs" :key="index">
          <div class="label flex items-center justify-between mb-2">
            <p class="text-lg font-medium text-gray-800">{{ blog.title }}</p>
            <div>
              <span v-if="showContent === index"
                ><i
                  class="fa-solid fa-minus"
                  @click="toggleAccordion(index)"
                ></i
              ></span>
              <span v-else
                ><i class="fa-solid fa-plus" @click="toggleAccordion(index)"></i
              ></span>
            </div>
          </div>
          <div class="content grid gap-3" v-if="showContent === index">
            <span class="text-sm text-gray-700 font-medium italic">{{
              blog.text
            }}</span>
            <a :href="blog.url" class="btn w-fit" target="_blank">Read more</a>
          </div>
        </accordions>
      </div>
      <div class="flex items-center justify-center mt-20" v-else>
        <p class="text-lg text-gray-600 font-medium">
          Loading Blog contents...
        </p>
      </div>
    </div>
  </section>
</template>

<script>
import accordions from "~/components/accordions.vue";
export default {
  components: { accordions },
  data() {
    return {
      showContent: null,
      blogs: [
        {
          name: "nuxt-app",
          private: true,
          type: "module",
          scripts: {
            build: "nuxt build",
            dev: "nuxt dev",
            generate: "nuxt generate",
            preview: "nuxt preview",
            postinstall: "nuxt prepare",
            "json-server": "json-server --watch db.json --port 3001",
          },
          devDependencies: {
            "@nuxtjs/tailwindcss": "^6.11.2",
            "json-server": "^1.0.0-alpha.23",
            nuxt: "^3.9.3",
            tailwindcss: "^3.4.1",
            vue: "^3.4.14",
            "vue-router": "^4.2.5",
          },
        },
      ],
    };
  },
  mounted() {
    fetch("http://localhost:3001/blogs")
      .then((res) => res.json())
      .then((data) => (this.blogs = data))
      .catch((err) => console.log(err.message));
  },
  methods: {
    toggleAccordion(index) {
      this.showContent = this.showContent === index ? null : index;
    },
  },
};
</script>

<style></style>
