<template>
  <!-- Navbar -->
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

  <div class="container mx-auto p-6 mt-10">
    <div class="flex flex-col space-y-4 items-center text-center">
      <h2 class="text-7xl font-medium text-gray-500">about.</h2>
      <span class="font-medium text-gray-500"
        >I'm a frontend engineer based in Lagos, Nigeria.</span
      >

      <p class="text-gray-500 w-[80%]">
        Embarking on my professional journey, I initially found myself in the
        classroom as a school teacher at a primary school. Later, driven by a
        curiosity to explore new horizons, I enrolled at Adekunle Ajasin
        University, Akungba, Ondo state, where I pursued a degree in Sociology.
      </p>

      <p class="text-gray-500 w-[80%]">
        Post-university, I completed my National Youth Service Corps (NYSC) in
        2020 and returned to Lagos. It was here that I ventured into the dynamic
        world of technology. Joining a startup as a customer success officer, I
        marveled at the feats accomplished by our Chief Technology Officer
        (CTO). His ability to navigate the tech landscape, transforming what
        seemed impossible into reality, fascinated me.
      </p>

      <p class="text-gray-500 w-[80%]">
        My entry into the tech space took a decisive turn when a friend named
        Michael introduced me to UI/UX design through insightful videos. This
        introduction marked the beginning of my exploration and immersion into
        the tech world.
      </p>

      <p class="text-gray-500 w-[80%]">
        From my humble beginnings as a school teacher to navigating the realms
        of technology, my journey has been one of continuous learning and
        adaptation. I am now eager to contribute my unique perspective and
        skills to the ever-evolving tech landscape.
      </p>
    </div>
  </div>

  <!-- =============footer section================ -->
  <section>
    <div class="container mx-auto grid items-center p-6 text-center">
      <small>©2024 theolukayodeasemudara.com</small>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style></style>
