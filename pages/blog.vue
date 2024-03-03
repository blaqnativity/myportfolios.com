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

      <div class="mt-20 grid gap-4">
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
            <a :href="blog.url" class="btn w-fit">Read more</a>
          </div>
        </accordions>
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
          title: "Slots VS Props in NUXT-3",
          text: "With Slots, you can easily display and maneuver the contents of a component, i.e; form, modal and many others...",
          url: "https://dev.to/theolukayodeasemudara/slots-vs-props-in-nuxt-3-34h8",
        },
        {
          title: "Your First Nuxt App",
          text: "Building apps with NUXT makes your work very easy and seamless especially cause of the fact that NUXT has done so many stuffs behind the scenes for you unlike Vuejs where you have to fix most yourself.",
          url: "https://dev.to/theolukayodeasemudara/your-first-nuxt-3-app-22c",
        },
      ],
    };
  },
  methods: {
    toggleAccordion(index) {
      this.showContent = this.showContent === index ? null : index;
    },
  },
};
</script>

<style></style>
