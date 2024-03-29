<script setup>
const router = useRouter();

const gotToCareers = () => {
  router.push({ path: "/Careers/Application" });
};
const gotoAbout = () => {
  router.push({ path: "/About" });
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

        <button class="btnMain mr-6" @click="gotToCareers">Apply Now</button>
        <button class="btnOutline" @click="gotoAbout">About Us</button>
      </div>
      <!-- right div -->
      <div>
        <img src="/assets/img/time.jpg" alt="" />
      </div>
    </div>
  </section>
</template>
