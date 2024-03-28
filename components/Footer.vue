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
  { name: "Services", url: "/services" },
  { name: "Careers", url: "/career" },
];
</script>

<template>
  <div class="mt-20 w-full h-[5rem] bottom-0 right-0 border-t-0.5 z-50">
    <div class="container mx-auto p-6 flex justify-center items-center h-full">
      <ul class="flex flex-col md:flex-row space-x-12 items-center">
        <NuxtLink
          :to="link.url"
          class="font-medium leading-8 tracking-wide text-gray-600 hover:text-orange-600 transition-all duration-150"
          v-for="link in links"
          :key="link"
          >{{ link.name }}</NuxtLink
        >
        <button class="btnOutline" @click="handleClick">Contact Us</button>
      </ul>
    </div>
  </div>
</template>
