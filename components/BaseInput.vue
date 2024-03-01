<template>
  <div class="backdrop">
    <form @click.prevent>
      <div class="flex items-center justify-between">
        <h2>{{ title }}</h2>
        <span
          ><i class="fa-regular fa-square-minus" @click="closeForm"></i
        ></span>
      </div>
      <label>Name:</label>
      <input type="text" />

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
</template>

<script>
export default {
  props: ["title"],
  data() {
    return {};
  },
  methods: {
    closeForm() {
      this.$emit("close");
    },
  },
};
</script>

<style scoped>
/* input styles */
input,
textarea {
  @apply p-2;
}

/* contact form */
form {
  @apply w-[420px] bg-white text-left p-[40px] rounded-md border mx-auto my-10;
}

form label {
  @apply text-[#aaa] inline-block mt-[25px] mb-0 mr-[15px] uppercase text-[.6em] font-bold;
}

form input {
  @apply block py-[10px] px-[6px] w-[100%] box-border  border-b-[1px] text-[#555] outline-none;
}

form textarea {
  @apply block py-[10px] px-[6px] w-[100%] box-border border-b-[1px] text-[#555] outline-none;
}
</style>
