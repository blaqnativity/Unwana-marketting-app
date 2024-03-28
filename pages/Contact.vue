<script setup>
definePageMeta({
  layout: "custom",
});

const showSignup = ref(true);
</script>

<template>
  <section class="h-screen-[5rem] space-y-10">
    <div class="text-center mt-20">
      <h2 class="subLead">Create an Account</h2>
      <p class="sub-text">Already have an account? <span>Sign in</span></p>
    </div>
    <div v-if="showSignup">
      <Signup />
    </div>
    <div v-else>
      <Login />
    </div>
  </section>
</template>

<style>
input {
  @apply outline-none text-sm font-bold text-gray-500 py-3 px-1 bg-transparent border-b-2 border-gray-300;
}

label {
  @apply text-xl font-semibold text-gray-600;
}
</style>
