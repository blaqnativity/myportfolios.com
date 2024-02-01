<template>
  <!-- ==============Navbar Section=============== -->
  <nav class="relative container mx-auto p-6">
    <div class="flex items-center justify-between">
      <!-- Logo -->
      <NuxtLink to="/"
        ><span class="text-lg md:text-2xl">olukayode!</span></NuxtLink
      >

      <!-- Menu Items -->
      <ul class="hidden nav-links md:flex space-x-6 items-center">
        <NuxtLink to="/"><span>About me</span></NuxtLink>
        <NuxtLink to="/"><span>Dev Projects</span></NuxtLink>
        <NuxtLink to="/"><span>Contact</span></NuxtLink>
      </ul>
    </div>
  </nav>

  <!-- =============Hero Section================== -->
  <section class="mt-20 mb-32">
    <!-- ====================flex container===================== -->
    <div
      class="container flex flex-col-reverse items-center px-6 mx-auto mt-10 space-y-0 md:space-y-0 md:flex-row"
    >
      <!-- left item -->
      <div class="mt-10 flex flex-col space-y-6 md:w-1/2 md:mt-0">
        <span class="max-w-sm text-center md:text-left"
          >HELLO, I'M Olukayode Asemudara</span
        >
        <h1
          class="max-w-lg text-4xl font-bold text-center md:text-5xl md:text-left"
        >
          I build web/mobile friendly Interfaces.
        </h1>
        <p class="text-center md:text-left font-medium text-gray-600">
          Junior frontend Engineer
        </p>
        <div class="flex justify-center md:justify-start">
          <NuxtLink to="/"
            ><button class="btn px-6 py-3 border-2 border-gray-700 font-medium">
              Hire me
            </button></NuxtLink
          >
        </div>
      </div>
      <!-- image -->
      <div class="items-center md:items-end md:w-1/2">
        <img src="~/assets/img/hero.svg" alt="" />
      </div>
    </div>
  </section>

  <!-- ================About section================ -->
  <section class="mb-32">
    <div class="container mx-auto px-6">
      <div class="title flex flex-col space-y-6 text-center">
        <h4 class="grayTitle text-gray-600 font-medium text-xl">About</h4>
        <h3 class="font-medium text-2xl text-gray-700">My Story.</h3>
      </div>

      <div
        class="flex flex-col-reverse items-center mt-20 md:flex-row gap-10 md:gap-20"
      >
        <!-- items-left -->
        <div class="md:w-1/2">
          <img src="~/assets/img/about.svg" alt="" />
        </div>
        <!-- items-right -->
        <div class="md:w-1/2">
          <p class="mb-2">
            Junior Frontend Engineer that loves creating solutions and crafting
            amazing user experiences.
          </p>
          <p class="mb-2">
            My journey with Software development started in 2021, when I joined
            Medipalhealthcare as a customer success officer in January. I used
            to accompany my CTO to facilities that used our solutions for
            medical purposes and during that period, I saw how he used to edit
            HTML tags and contents of the software from a supposed backend.
          </p>
          <p class="mb-2">
            I was pretty impressed and wanted to give it a try too. A friend by
            the name Micheal(UI/UX expert), asked me to watch some couple of
            videos on youtube and that was the push I needed. Over the years, I
            have taught myself how to write some stacks following youtube aided
            videos and Udemy materials too.
          </p>
          <p class="mb-2">
            Currently, I'm actively searching for my next role where I can keep
            adding value and working with amazing people. Feel free to reach out
            if you have an opening that fits my skillset or not - I'm open to
            learning
          </p>
        </div>
      </div>
    </div>
  </section>

  <!-- ================Skills Section=============== -->
  <section class="mb-32">
    <div class="container mx-auto px-6 space-y-6">
      <div class="flex flex-col space-y-4 items-center">
        <h4 class="grayTitle text-gray-600 font-medium text-xl">Skills</h4>
        <h2 class="font-medium text-2xl text-gray-700">Tech Stack.</h2>
        <p>I have experience working with the following technologies</p>
      </div>

      <div class="flex flex-wrap items-center justify-center gap-6">
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">HTML</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">CSS</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl"
          >Javascript (ES6)</span
        >
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Tailwindcss</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Bootstrapcss</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Figma</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Canva Design</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Webflow</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Wordpress</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Netlify</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Git</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Excel</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Power Point</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl"
          >Microsoft Word</span
        >
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style></style>
