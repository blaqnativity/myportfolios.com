<template>
  <!-- ==============Navbar Section=============== -->
  <section class="fixed top-0 backdrop-blur-sm w-[100%] shadow-md">
    <nav
      class="relative container mx-auto p-4 flex justify-between items-center z-20"
    >
      <div class="flex items-center">
        <span><i class="fa-brands fa-hashnode"></i></span>
        <NuxtLink class="logo" to="/">{{ logo }}</NuxtLink>
      </div>

      <!-- nav menu -->
      <ul class="main_menu hidden space-x-10 md:flex">
        <li v-for="link in links" :key="link.url">
          <NuxtLink :to="link.url">{{ link.text }}</NuxtLink>
        </li>
      </ul>

      <div class="block md:hidden" @click="toggleBtn">
        <i class="fa-regular fa-square-minus" v-if="showMenu"></i>
        <i class="fa-solid fa-bars" v-else></i>
      </div>

      <div class="dropdown_menu" v-if="showMenu">
        <ul class="main_menu space-x-10 md:flex">
          <!-- Remove md:hidden class -->
          <li v-for="link in links" :key="link.url">
            <NuxtLink :to="link.url">{{ link.text }}</NuxtLink>
          </li>
        </ul>
      </div>
    </nav>
  </section>
</template>

<script>
export default {
  data() {
    return {
      showMenu: false,
      logo: "Olukayode!",
      links: [
        { text: "About", url: "/about" },
        { text: "Portfolio", url: "/" },
        { text: "Blog", url: "/blog" },
      ],
    };
  },
  methods: {
    toggleBtn() {
      this.showMenu = !this.showMenu;
    },
  },
};
</script>

<style></style>
