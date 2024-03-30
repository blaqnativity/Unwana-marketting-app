<template>
  <footer class="container text-gray-500 px-4 py-5 max-w-screen-xl mx-auto">
    <div class="max-w-lg sm:mx-auto sm:text-center">
      <p class="subLead">Unwana Wave Marketting</p>
    </div>
    <ul
      class="items-center justify-center mt-8 space-y-5 sm:flex sm:space-x-4 sm:space-y-0"
    >
      <li v-for="item in footerNavs" :key="item.id" class="hover:text-gray-800">
        <a href="{{item.href}}">
          {{ item.name }}
        </a>
      </li>
    </ul>
    <div class="mt-8 justify-center sm:flex">
      <div class="mt-4 sm:mt-0">&copy; 2024 Unwana All rights reserved.</div>
    </div>
  </footer>
</template>

<script setup>
const footerNavs = [
  {
    href: "javascript:void()",
    name: "About",
  },
  {
    href: "javascript:void()",
    name: "Blog",
  },
  {
    href: "javascript:void()",
    name: "",
  },
  {
    href: "javascript:void()",
    name: "Team",
  },
  {
    href: "javascript:void()",
    name: "Careers",
  },
];
</script>

<style scoped>
.svg-icon path,
.svg-icon polygon,
.svg-icon rect {
  fill: currentColor;
}
</style>
