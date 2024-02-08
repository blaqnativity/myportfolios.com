<template>
  <!-- section page -->
  <section>
    <div class="container mx-auto p-6 mt-20">
      <div class="flex flex-col space-y-4">
        <p>Send me a mail</p>
        <h2 class="font-medium text-2xl text-gray-700">Contact me here</h2>
        <div class="w-[20%] bg-gray-400 h-1 rounded-full"></div>
      </div>

      <div class="flex flex-col items-center gap-4 mt-20 md:flex-row">
        <div class="w-[80%] md:w-[50%]">
          <img src="~/assets/img/mail.svg" alt="" />
        </div>
        <div class="form w-[80%] rounded-md shadow-sm border md:w-1/2">
          <form class="p-6 flex flex-col space-y-4">
            <p>Get in touch</p>
            <div class="flex flex-col space-y-2">
              <label>Name</label>
              <input type="text" class="outline-none border-b-2" required />
            </div>
            <div class="flex flex-col space-y-2">
              <label>email</label>
              <input type="email" class="outline-none border-b-2" required />
            </div>
            <div class="flex flex-col gap-2">
              <label>Your message</label>
              <textarea
                name="message"
                rows="5"
                cols="30"
                class="outline-none border rounded-md"
              ></textarea>
            </div>

            <div>
              <button class="btn flex items-center gap-2">
                Send <i class="fa-regular fa-paper-plane"></i>
              </button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style></style>
