<script setup>
const goHome = () => {
  navigateTo("/");
  // router.push({ path: "/" });
};

const handleClick = () => {
  navigateTo("/contact");
};

const links = [
  { name: "About", url: "/about" },
  { name: "Services", url: "/services" },
  { name: "Careers", url: "/careers" },
];
</script>

<template>
  <div class="w-full h-[5rem] sticky top-0 right-0 shadow-md z-50 bg-gray-50">
    <div class="container mx-auto p-6 flex justify-between items-center h-full">
      <div class="logo">
        <span
          class="md:text-2xl font-bold leading-10 text-orange-600 tracking-wider uppercase cursor-pointer"
          @click="goHome"
          >Unwana</span
        >
      </div>

      <ul class="flex flex-col md:flex-row space-x-12 items-center">
        <NuxtLink
          :to="link.url"
          class="font-medium leading-8 tracking-wide text-gray-600 hover:text-orange-600 md:hover:bg-orange-100 md:px-3 md:py-1 rounded-full transition-all duration-150"
          v-for="link in links"
          :key="link"
          >{{ link.name }}</NuxtLink
        >
        <button class="btnMain" @click="handleClick">Contact Us</button>
      </ul>
    </div>
  </div>
</template>
