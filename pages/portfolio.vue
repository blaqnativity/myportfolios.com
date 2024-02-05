<template>
  <!-- ================Projects section================ -->
  <section class="mb-32">
    <div class="container mx-auto px-6">
      <div class="title flex flex-col space-y-6 text-start">
        <h4 class="grayTitle text-gray-600 font-medium text-xl">Projects</h4>
        <h3 class="font-medium text-2xl text-gray-700">Featured Projects.</h3>
      </div>

      <!-- flex containers -->
      <div class="flex flex-col space-y-10">
        <!-- flex items -->
        <div class="flex flex-col md:flex-row gap-8 mt-10">
          <div>
            <img src="~/assets/img/projectone.png" alt="" />
          </div>
          <div class="flex flex-col gap-4">
            <NuxtLink
              ><h3 class="text-xl font-semibold text-gray-700">
                Tom's Purse
              </h3></NuxtLink
            >
            <p>
              Tom's purse is a friendly e-wallet system that allows you save
              money in little bits with ease just like the kolo system of old
              days.
            </p>
            <span class="text-gray-600 text-sm"
              >One of my first tasks using tailwindcss.</span
            >
            <NuxtLink to="/" class="btnLine">View More</NuxtLink>
          </div>
        </div>
        <div class="flex flex-col md:flex-row gap-8 my-8">
          <div>
            <img src="~/assets/img/projecttwo.png" alt="" />
          </div>
          <div class="flex flex-col gap-4">
            <NuxtLink
              ><h3 class="text-xl font-semibold text-gray-700">
                olukayodetaiwo.netlify.app
              </h3></NuxtLink
            >
            <p>
              Its one of my first personal portfolio made with bootstrap css and
              a few javascript lines. The best thing I loved bout this was the
              way it was designed unlike the regular kind of personal portfolio.
            </p>
            <span class="text-gray-600 text-sm">Made with bootstrapcss.</span>

            <NuxtLink to="/" class="btnLine">View More</NuxtLink>
          </div>
        </div>
        <div class="flex flex-col md:flex-row gap-8 my-8">
          <div>
            <img src="~/assets/img/projectthree.png" alt="" />
          </div>
          <div class="flex flex-col gap-4">
            <NuxtLink
              ><h3 class="text-xl font-semibold text-gray-700">
                Amorestore
              </h3></NuxtLink
            >
            <p>
              Its a typify I created while I was learning how to merge Nuxt3,
              Vuejs and Tailwindcss knowledges all together to create one
              e-commerce store. I managed to integrate in it a commerce api
              also.
            </p>
            <span class="text-gray-600 text-sm"
              >Journey using Nuxt3, Vuejs and Bootstrap css all together.</span
            >

            <NuxtLink to="/" class="btnLine">View More</NuxtLink>
          </div>
        </div>
      </div>

      <!-- flex containers -->
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style></style>
