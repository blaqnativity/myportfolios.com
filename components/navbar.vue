<template>
  <!-- ==============Navbar Section=============== -->
  <nav class="relative container mx-auto p-6">
    <div class="flex items-center justify-between">
      <!-- Logo -->
      <NuxtLink to="/"
        ><span class="logo text-4xl md:text-5xl font-medium"
          >olukayode!</span
        ></NuxtLink
      >

      <!-- Menu Items -->
      <ul
        class="hidden md:flex space-x-6 items-center text-gray-600 text-sm uppercase font-semibold"
      >
        <NuxtLink to="about" class="hover:text-gray-400"
          ><span>About me</span></NuxtLink
        >
        <NuxtLink to="/" class="hover:text-gray-400"
          ><span>Dev Projects</span></NuxtLink
        >
        <NuxtLink to="/" class="hover:text-gray-400"
          ><span>Contact</span></NuxtLink
        >
      </ul>

      <!-- hamburger icon -->
      <div
        class="hamburgerBtn md:hidden cursor-pointer space-y-1"
        @click="toggle()"
      >
        <div class="w-8 h-0.5 bg-black"></div>
        <div class="w-8 h-0.5 bg-black"></div>
        <div class="w-8 h-0.5 bg-black"></div>
      </div>

      <!-- hamburger menu -->
      <ul
        class="menu hidden items-center flex-col absolute left-0 w-full top-0 p-10 rounded-b-3xl text-sm uppercase font-semibold bg-indigo-500 space-y-4 text-white"
      >
        <NuxtLink to="/"><span>About me</span></NuxtLink>
        <NuxtLink to="/"><span>Dev Projects</span></NuxtLink>
        <NuxtLink to="/"><span>Contact</span></NuxtLink>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style></style>
