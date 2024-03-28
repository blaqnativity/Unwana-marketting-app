<script setup>
const goHome = () => {
  navigateTo("/");
  // router.push({ path: "/" });
};

const handleClick = () => {
  navigateTo("/contact");
  // router.push({ path: "/contact" });
};

const links = [
  { name: "About", url: "/about" },
  { name: "Services", url: "/services" },
  { name: "Careers", url: "/career" },
];
</script>

<template>
  <div class="w-full h-[5rem] sticky top-0 right-0 shadow-md z-50 bg-white">
    <div class="container mx-auto p-6 flex justify-between items-center h-full">
      <div class="logo">
        <span
          class="md:text-3xl font-bold leading-10 text-orange-600 tracking-wider uppercase cursor-pointer"
          @click="goHome"
          >Unwana</span
        >
      </div>

      <ul class="flex flex-col md:flex-row space-x-12 items-center">
        <NuxtLink
          :to="link.url"
          class="font-medium leading-8 tracking-wide text-gray-600 hover:text-orange-600 transition-all duration-150"
          v-for="link in links"
          :key="link"
          >{{ link.name }}</NuxtLink
        >
        <button class="btnMain" @click="handleClick">Get Started</button>
      </ul>
    </div>
  </div>
</template>
