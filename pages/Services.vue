<script setup>
const router = useRouter();
useHead({
  title: "Uwana",
});

const handleClick = () => {
  router.push({ path: "/About" });
  // navigateTo("/About");
};

const scrollTo = () => {
  scrollTo("/");
};
</script>

<template>
  <!-- hero section -->
  <section class="h-screen-[5rem]">
    <div class="grid grid-cols-1 md:grid-cols-2 h-full items-center gap-10">
      <!-- left div -->
      <div class="space-y-6">
        <h2 class="lead">Elevate Impact through Strategic Engagement</h2>
        <p class="sub-text">
          Empowering Non-Profits and Businesses to Forge Lasting Connections,
          Drive Sales, and Achieve Remarkable Growth
        </p>

        <button class="btnOutline" @click="handleClick">About Us</button>

        <span
          class="block cursor-pointer text-sm font-medium text-gray-600"
          @click="scrollTo"
          >Scroll down to explore</span
        >
      </div>
      <!-- right div -->
      <div>
        <img src="/assets/img/marketting.jpg" alt="" />
      </div>
    </div>
  </section>

  <!-- cta section -->
  <section class="mt-36 text-center grid items-center">
    <div class="space-y-8 text-center">
      <h2 class="titleText">Welcome to Unwana Marketing</h2>
      <p class="sub-text">
        Here are the services offered by Fortis Wave Marketing
      </p>
    </div>
  </section>
</template>
