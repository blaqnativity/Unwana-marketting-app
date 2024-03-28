<script setup>
const router = useRouter();

const goHome = () => {
  router.push({ path: "/" });
};
</script>

<template>
  <section class="w-full h-screen">
    <div class="h-full flex flex-col justify-center items-center space-y-20">
      <img src="~/assets/img/404.png" alt="" />
      <p class="text-sm uppercase text-gray-500 font-medium">
        Page cannot be found
      </p>
      <button class="btnOutline" @click="goHome">Back to Home</button>
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
