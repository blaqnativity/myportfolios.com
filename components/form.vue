<template>
  <!-- contact form -->
  <div class="form">
    <form @submit.prevent="formInput">
      <h2>Send Olukayode a DM</h2>
      <label>Name:</label>
      <input type="text" />

      <label>Email:</label>
      <input type="email" />

      <label>Message:</label>
      <textarea name=""></textarea>

      <button class="btn flex items-center gap-2 mt-4" @click="submitForm">
        <span>Send Message</span>
        <i class="fa-regular fa-paper-plane"></i>
      </button>
    </form>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
