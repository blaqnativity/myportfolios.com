<template>
  <!-- =============Hero Section================== -->
  <section class="mt-40 flex h-[100vh-89.59px] justify-center">
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
          <button class="btn" @click="toggleForm">Hire me</button>
        </div>

        <div class="backdrop" v-if="showForm">
          <form @click.prevent>
            <div class="flex items-center justify-between">
              <h2>{{ title }}</h2>
              <span
                ><i class="fa-regular fa-square-minus" @click="closeForm"></i
              ></span>
            </div>

            <label>Email:</label>
            <input type="email" />

            <label>Message:</label>
            <textarea name=""></textarea>

            <button class="btn flex items-center gap-2 mt-4">
              <span>Send Message</span>
              <i class="fa-regular fa-paper-plane"></i>
            </button>
          </form>
        </div>
      </div>
      <!-- image -->
      <div class="items-center md:items-end md:w-1/2">
        <img src="~/assets/img/hero.svg" alt="" />
      </div>
    </div>
  </section>

  <!-- whatsapp icon -->
  <whatsapp />

  <!-- ================Contact section================ -->
</template>

<script>
import BaseInput from "~/components/BaseInput.vue";
import whatsapp from "~/components/sticky-components/whatsapp.vue";
export default {
  components: { BaseInput, whatsapp },
  data() {
    return {
      title: "Send me a message",
      showForm: false,
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

<style>
.backdrop {
  bottom: 0;
  right: 0;
  position: fixed;
  background: rgba(0, 0, 0, 0.5);
  height: 100%;
  width: 100vw;
  z-index: 10;
}
</style>
