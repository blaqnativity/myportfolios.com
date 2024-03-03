<template>
  <div class="backdrop">
    <slot></slot>
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
