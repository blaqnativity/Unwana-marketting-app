<script setup>
const error = useError();

const goHome = () => {
  navigateTo("/");
};
</script>

<template>
  <section class="w-full h-screen text-center">
    <div class="h-full flex flex-col justify-center items-center space-y-10">
      <img class="h-60 w-auto" src="~/assets/img/404.png" alt="" />
      <div
        class="space-y-10 items-center text-center shadow-lg w-1/3 py-10 border rounded-lg"
      >
        <h2 class="text-2xl text-orange-600 font-sans font-semibold">
          Error: {{ error.statusCode }}
        </h2>
        <p class="text-sm uppercase text-gray-500 font-medium">
          {{ error.message }}
        </p>
        <button class="btnOutline" @click="goHome">Back to Home</button>
      </div>
    </div>
  </section>
</template>

<style>
div {
  /* background-image: url(~/assets/img/bg-img.png);
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center; */
}
</style>
