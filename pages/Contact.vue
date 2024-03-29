<script setup></script>

<template>
  <!-- hero section -->
  <section class="h-screen-[5rem]">
    <div class="grid grid-cols-1 md:grid-cols-2 h-full items-center gap-10">
      <!-- left div -->
      <div class="space-y-6">
        <h2 class="lead">How can we help? ></h2>
        <p class="sub-text">
          Let us help by answering any questions you may have
        </p>

        <button class="btnMain mr-6" @click="appForm">Careers</button>
        <button class="btnOutline" @click="goTo">About Us</button>

        <span
          class="block cursor-pointer text-sm font-medium text-gray-600"
          @click="scrollTo"
          >Scroll down to explore</span
        >
      </div>
      <!-- right div -->
      <div>
        <img src="/assets/img/contact.jpg" alt="" />
      </div>
    </div>
  </section>

  <!-- contact form -->
  <section class="mt-32">
    <div class="text-center space-y-4 w-1/2 mx-auto">
      <h2 class="subLead">Send us a message</h2>
      <p class="sub-text">
        Let us help you with any questions you may have. We are here to help you
        grow your business
      </p>
    </div>

    <form class="space-y-8 mt-20">
      <BaseInput label="Full name" type="text" required />
      <BaseInput label="Email" type="email" required />
      <BaseInput label="Subject" type="text" />
      <div class="space-y-2 mt-2 text-start">
        <Label>Your message</Label>
        <Textmsg />
      </div>

      <button
        class="bg-orange-600 text-bold font-lg text-white px-4 py-2 rounded-full hover:bg-orange-500 transition-all duration-150"
      >
        Send message
      </button>
    </form>
  </section>
</template>

<style></style>
