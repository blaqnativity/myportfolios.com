<template>
  <!-- ==============Navbar Section=============== -->
  <section class="fixed top-0 backdrop-blur-sm w-[100%] shadow-md">
    <nav
      class="relative container mx-auto p-4 flex justify-between items-center z-10"
    >
      <div>
        <NuxtLink class="logo" to="/">{{ logo }}</NuxtLink>
      </div>

      <!-- nav menu -->
      <ul class="main_menu hidden space-x-10 md:flex">
        <li>
          <NuxtLink to="/about">{{ link1 }}</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/portfolio">{{ link2 }}</NuxtLink>
        </li>
      </ul>

      <div class="block md:hidden" @click="toggleBtn">
        <i class="fa-regular fa-square-minus" v-if="showMenu"></i>
        <i class="fa-solid fa-bars" v-else></i>
      </div>

      <div class="dropdown_menu" v-if="showMenu">
        <li>
          <NuxtLink to="/about">{{ link1 }}</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/">{{ link2 }}</NuxtLink>
        </li>
      </div>
    </nav>
  </section>
</template>

<script>
export default {
  data() {
    return {
      showMenu: false,
      logo: "olukayode!",
      link1: "About me",
      link2: "Portfolio",
    };
  },
  methods: {
    toggleBtn() {
      console.log("menu button clicked");
      this.showMenu = !this.showMenu;
    },
  },
};
</script>

<style></style>
