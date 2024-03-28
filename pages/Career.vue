<script setup>
const router = useRouter();
useHead({
  title: "Uwana",
});

const handleClick = () => {
  router.push({ path: "/About" });
  // navigateTo("/About");
};
</script>

<template>
  <!-- hero section -->
  <section class="h-screen-[5rem]">
    <div class="grid grid-cols-1 md:grid-cols-2 h-full items-center gap-10">
      <!-- left div -->
      <div class="space-y-6">
        <h2 class="lead">Join our team today</h2>
        <p class="sub-text">
          Join us at FortisWave Marketing, where you'll have the opportunity to
          work with inspiring colleagues, grow both personally and
          professionally, and be part of a purpose-driven organization that's
          making waves in the marketing industry and beyond. Together, let's
          make a lasting impact and build a brighter future.
        </p>

        <button class="btnOutline" @click="handleClick">About Us</button>

        <!-- <span
          class="block cursor-pointer text-sm font-medium text-gray-600"
          @click="scrollTo"
          >Scroll down to explore</span
        > -->
      </div>
      <!-- right div -->
      <div>
        <img src="/assets/img/joinus.jpg" alt="" />
      </div>
    </div>
  </section>
</template>
