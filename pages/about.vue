<template>
  <div class="container mx-auto p-6">
    <!-- about text head -->
    <section class="mt-20">
      <div
        class="flex flex-col space-y-4 items-center text-center justify-center"
      >
        <span class="font-medium text-gray-500">Get to know me</span>
        <h2 class="text-5xl font-medium text-gray-500 md:text-7xl">about.</h2>

        <p class="text-gray-500 w-[80%]">
          Olukayode is a Software Engineer, Olukayode has two years experience
          providing front-end development, producing high quality responsive
          websites, cross platform mobile-apps and exceptional user experience.
        </p>

        <p class="text-gray-500 w-[80%]">
          The work he provides is of highest quality, fully responsive, and
          tested in a wide range of devices. He takes great care to ensure each
          project is well-documented and easily maintainable so you can enhance
          a website as your company grows.
        </p>

        <div class="mt-14">
          <button class="btn">Download Resume</button>
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
      <div class="grid items-center justify-center mt-10 gap-4 md:grid-cols-2">
        <div class="card flex justify-center">
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
              Kay did an excellent creative job, addressing our request quickly,
              and also providing her own graphic insight, being open to feedback
              and changes or edits when they arose. She worked with us the
              entire way. Highly recommended.
            </p>
          </div>
        </div>
        <div class="card flex justify-center">
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
              Kayode did an excellent creative job, addressing our request
              quickly, and also providing her own graphic insight, being open to
              feedback and changes or edits when they arose. She worked with us
              the entire way. Highly recommended.
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- contact me -->
    <section class="mt-32">
      <div class="container mx-auto px-6">
        <div class="title flex flex-col space-y-6 text-center">
          <h4 class="grayTitle text-gray-600 font-medium text-xl">Contact</h4>
          <h3 class="font-medium text-2xl text-gray-700">
            Are you ready to work with me?
          </h3>
        </div>

        <div
          class="flex flex-col items-center md:flex-row mt-20 md:space-x-20 space-y-10"
        >
          <!-- items-left -->
          <div class="md:w-1/2">
            <img src="~/assets/img/contact.svg" alt="" />
          </div>
          <!-- items right -->
          <div class="text-center md:text-left">
            <p class="mb-4">
              I'm actively open to new opportunities and requests.
            </p>
            <p>
              If you have a question, or just want to say hi, I'll try my best
              to get back to you.
            </p>

            <div class="flex justify-center md:justify-start mt-6">
              <button class="btn" @click="toggleForm">Get in touch</button>
            </div>

            <!-- form component using slot -->
            <div class="backdrop" v-if="showForm">
              <form @click.prevent>
                <div class="flex items-center justify-between">
                  <h2>{{ title }}</h2>
                  <span
                    ><i
                      class="fa-regular fa-square-minus"
                      @click="closeForm"
                    ></i
                  ></span>
                </div>

                <label>Email:</label>
                <input type="email" />

                <div>
                  <label for="selectInput">Hire my services for:</label>
                  <select id="selectInput" v-model="selectedOption">
                    <option value="">Select One</option>
                    <option
                      v-for="(option, index) in options"
                      :key="index"
                      :value="option.value"
                    >
                      {{ option.label }}
                    </option>
                  </select>
                  <p v-if="selectedOption">
                    You selected: {{ selectedOption }}
                  </p>
                </div>

                <label>Message:</label>
                <textarea name=""></textarea>

                <button class="btn flex items-center gap-2 mt-4">
                  <span>Send Message</span>
                  <i class="fa-regular fa-paper-plane"></i>
                </button>
              </form>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>

  <!-- ================Skills Section=============== -->
  <section class="mt-20 mb-10">
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
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Vue-JS</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">NUXT-3</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Tailwindcss</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Bootstrapcss</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Figma</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Adobe XD</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Canva Design</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Webflow</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Wordpress</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Netlify</span>
        <span class="pill bg-blue-200 px-5 py-2 rounded-xl">Git</span>
      </div>
    </div>
  </section>
</template>

<script>
import footerView from "~/components/footerView.vue";
export default {
  components: { footerView },
  data() {
    return {
      showForm: false,
      selectedOption: "",
      options: [
        { label: "Wordpress", value: "Wordpress Sites" },
        { label: "Design", value: "UI Designs" },
        { label: "Frontend", value: "Code Development" },
        // Add more options as needed
      ],
    };
  },
  methods: {
    toggleForm() {
      this.showForm = !this.showForm;
    },
    closeForm() {
      this.showForm = !this.showForm;
    },
  },
};
</script>

<style></style>
