<script setup>
const showSignup = ref(true);

const toggleForm = () => {
  showSignup.value = !showSignup.value;
};
</script>

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
</template>

<style></style>
