<template>
  <!-- ==============Navbar Section=============== -->
  <section class="w-[100%] shadow-md">
    <nav
      class="relative container mx-auto p-4 flex justify-between items-center"
    >
      <div>
        <NuxtLink class="logo" to="/">olukayode!</NuxtLink>
      </div>

      <!-- nav menu -->
      <ul class="main_menu hidden space-x-10 md:flex">
        <li><NuxtLink to="/">About me</NuxtLink></li>
        <li><NuxtLink to="/">Portfolio</NuxtLink></li>
        <li><NuxtLink to="/">Contact</NuxtLink></li>
      </ul>

      <div class="togglebtn block md:hidden">
        <i class="fa-solid fa-bars"></i>
      </div>

      <div class="dropdown_menu">
        <li><NuxtLink to="/">About me</NuxtLink></li>
        <li><NuxtLink to="/">Portfolio</NuxtLink></li>
        <li><NuxtLink to="/">Contact</NuxtLink></li>
      </div>
    </nav>
  </section>
</template>

<script>
export default {};
</script>

<style></style>
