<script setup>
useHead({
  title: "Uwana",
});

const handleClick = () => {
  navigateTo("/About");
};
</script>

<template>
  <section class="h-screen-[5rem]">
    <div class="grid grid-cols-1 md:grid-cols-2 h-full items-center gap-10">
      <!-- left div -->
      <div class="w-3/4 space-y-6">
        <h2 class="lead">
          Fortis Wave Marketing -<span class="text-slate-900">
            Where Marketing Meets Purpose</span
          >
        </h2>
        <p class="sub-text">
          At FortisWave Marketing, we are a team of passionate individuals who
          thrive on connecting with people, building relationships, and driving
          success in a dynamic and diverse work environment.
        </p>

        <button class="btnOutline" @click="handleClick">About Us</button>
      </div>
      <!-- right div -->
      <div>
        <img src="/assets/img/hero.jpg" alt="" />
      </div>
    </div>
  </section>
</template>
