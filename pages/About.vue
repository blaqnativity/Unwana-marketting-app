<template>
  <!-- hero section -->
  <section class="h-screen-[5rem]">
    <div class="grid grid-cols-1 md:grid-cols-2 h-full items-center gap-10">
      <!-- left div -->
      <div class="space-y-6">
        <h2 class="lead">Get to know us -</h2>
        <p class="sub-text">
          As a company, we are committed to making a positive impact on the
          non-profit landscape throughout North America. We firmly believe that
          our results-oriented approach sets us apart and empowers our clients
          to achieve remarkable growth.
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
        <img src="/assets/img/time.jpg" alt="" />
      </div>
    </div>
  </section>
</template>
