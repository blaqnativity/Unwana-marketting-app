<script setup>
const back = () => {
  navigateTo("/");
};

definePageMeta({
  layout: "custom",
});

const showSignup = ref(true);

const toggleForm = () => {
  showSignup.value = !showSignup.value;
};
</script>

<template>
  <section class="h-screen-[5rem] space-y-6">
    <div class="text-center mt-10">
      <h2 class="subLead">Create an Account</h2>
    </div>
    <div v-if="showSignup">
      <Signup />
    </div>
    <div v-else>
      <Login />
    </div>

    <p class="sub-text text-center">
      <span v-if="showSignup"
        >Already have an account?
        <small
          class="text-orange-600 cursor-pointer text-lg"
          @click="toggleForm"
          >Login</small
        ></span
      >
      <span v-else
        >Don't have any?
        <small
          class="text-orange-600 cursor-pointer text-lg"
          @click="toggleForm"
          >Create one</small
        ></span
      >
    </p>
    <p class="sub-text text-center cursor-pointer" @click="back">
      Go back to home
    </p>
  </section>
</template>

<style></style>
