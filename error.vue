<script setup>
const error = useError();

const goHome = () => {
  navigateTo("/");
};
</script>

<template>
  <main
    class="grid h-screen place-items-center bg-white px-6 py-24 sm:py-32 lg:px-8"
  >
    <div class="text-center">
      <p class="text-base font-bold text-orange-600 w-[50%] mx-auto">
        Oooopssy!!!
      </p>
      <h1
        class="mt-4 text-3xl font-bold tracking-tight text-gray-900 sm:text-5xl"
      >
        {{ error.statusCode }}
      </h1>
      <p class="mt-6 text-base leading-7 text-gray-600">
        {{ error.message }}
      </p>
      <div class="mt-10 flex items-center justify-center gap-x-6">
        <button
          class="rounded-md bg-orange-600 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-orange-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
          @click="goHome"
        >
          Go back home
        </button>
        <a href="#" class="text-sm font-semibold text-gray-900"
          >Contact support <span aria-hidden="true">&rarr;</span></a
        >
      </div>
    </div>
  </main>
</template>
