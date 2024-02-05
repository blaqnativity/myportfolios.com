<template>
  <div class="container mx-auto p-6 mt-4">
    <!-- about text head -->
    <section>
      <div
        class="flex flex-col space-y-4 items-center text-center justify-center"
      >
        <span class="font-medium text-gray-500">Get to know me</span>
        <h2 class="text-5xl font-medium text-gray-500 md:text-7xl">about.</h2>

        <p class="text-gray-500 w-[80%]">
          Embarking on my professional journey, I initially found myself in the
          classroom as a school teacher at an early age. Later, driven by a
          curiosity to explore new horizons, I went on to have my first degree
          like every Nigerian child in Sociology at Adekunle Ajasin University,
          Akungba, Ondo State, Nigeria.
        </p>

        <p class="text-gray-500 w-[80%]">
          Joining a startup as a customer success officer, I marveled at the
          feats accomplished by our Chief Technology Officer (CTO). His ability
          to navigate the tech landscape, transforming what seemed impossible
          into reality, fascinated me.
        </p>

        <p class="text-gray-500 w-[80%]">
          From my humble beginnings as a school teacher to navigating the realms
          of technology, my journey has been one of continuous learning and
          adaptation. I am now eager to contribute my unique perspective and
          skills to the ever-evolving tech landscape.
        </p>

        <div class="mt-14">
          <button class="btn">Download CV</button>
        </div>
      </div>
    </section>

    <!-- services I offer -->
    <section>
      <div class="flex flex-col space-y-4 items-start justify-center mt-40">
        <p class="text-gray-500 font-medium">Services I offer to my clients</p>
        <h3 class="text-3xl font-medium">My Services</h3>
      </div>

      <!-- gird columns -->
      <div class="grid grid-cols-1 mt-20 gap-8 md:grid-cols-3">
        <!-- flex cards -->
        <div class="card">
          <img class="w-[30%]" src="~/assets/img/html.svg" alt="" />
          <h3>Front-end Development</h3>
          <p>
            I create responsive websites that allow the user to experience your
            website in the best and most appropriate way suited to the device
            they are using.
          </p>
        </div>
        <div class="card">
          <img class="w-[30%]" src="~/assets/img/web.svg" alt="" />
          <h3>Web Design</h3>
          <p>
            I have excellent understanding of graphic design, colour schemes,
            button design, interface design, Photoshop /Illustrator,
            navigational design.
          </p>
        </div>
        <div class="card">
          <img class="w-[30%]" src="~/assets/img/figma.svg" alt="" />
          <h3>UI/UX Design</h3>
          <p>
            I create user-friendly interfaces that enable users to understand
            how to use complex technical products.
          </p>
        </div>
        <div class="card">
          <img class="w-[30%]" src="~/assets/img/wordpress.svg" alt="" />
          <h3>Wordpress SIte Development</h3>
          <p>
            WordPress is the world’s most popular content management system
            which I have many years of experience with.
          </p>
        </div>
        <div class="card">
          <img class="w-[30%]" src="~/assets/img/rocket.svg" alt="" />
          <h3>Learn more</h3>
          <p>
            If you’d like to find out more about how I work and my process of
            working with clients, please send me a message in the contact page
            and give a little information about the project you have in mind.
          </p>
        </div>
      </div>
    </section>

    <!-- testimonials section -->
    <section>
      <div class="flex flex-col space-y-4 items-start justify-center mt-40">
        <p class="text-gray-500 font-medium">What my clients think about me</p>
        <h3 class="text-3xl font-medium">Testimonials</h3>
      </div>

      <!-- testimonial cards -->
      <div class="grid gap-8 md:grid-cols-2 mt-20">
        <div class="card">
          <div class="flex flex-col">
            <div class="flex items-start">
              <!-- client name / image -->
              <div class="flex items-center gap-2">
                <img class="w-[30%]" src="~/assets/img/avatar.svg" alt="" />
                <div class="flex flex-col items-start gap-2">
                  <h3>David Duru</h3>
                  <p>Founder Zicoma Operations</p>
                </div>
              </div>

              <div><i class="fa-solid fa-quote-right"></i></div>
            </div>
            <p class="mt-4">
              David did an excellent creative job, addressing our request
              quickly, and also providing her own graphic insight, being open to
              feedback and changes or edits when they arose. She worked with us
              the entire way. Highly recommended.
            </p>
          </div>
        </div>
        <div class="card">
          <div class="flex flex-col">
            <div class="flex items-start">
              <!-- client name / image -->
              <div class="flex items-center gap-2">
                <img class="w-[30%]" src="~/assets/img/avatar.svg" alt="" />
                <div class="flex flex-col items-start gap-2">
                  <h3>Phiona Williams</h3>
                  <p>Elite Homes Ltd</p>
                </div>
              </div>

              <div><i class="fa-solid fa-quote-right"></i></div>
            </div>
            <p class="mt-4">
              David did an excellent creative job, addressing our request
              quickly, and also providing her own graphic insight, being open to
              feedback and changes or edits when they arose. She worked with us
              the entire way. Highly recommended.
            </p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
