<script setup>
const back = () => {
  navigateTo("/");
};

definePageMeta({
  layout: "custom",
});

const showSignup = ref(true);
</script>

<template>
  <section class="h-screen-[5rem] space-y-10">
    <div class="text-center mt-10">
      <h2 class="subLead">Create an Account</h2>
      <p class="sub-text">Already have an account? <span>Sign in</span></p>
    </div>
    <div v-if="showSignup">
      <Signup />
    </div>
    <div v-else>
      <Login />
    </div>

    <p class="sub-text text-center cursor-pointer" @click="back">
      Go back to home
    </p>
  </section>
</template>

<style></style>
