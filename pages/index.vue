<script setup>
const router = useRouter()
useHead({
  title: 'Uwana',
})

const goTo = () => {
  router.push({ path: '/About' })
}
const appForm = () => {
  router.push({ path: '/careers/application' })
}
</script>

<template>
  <!-- hero section -->
  <section class="h-screen-[5rem]">
    <div class="grid grid-cols-1 md:grid-cols-2 h-full items-center gap-10">
      <!-- left div -->
      <div class="space-y-6">
        <h2 class="lead">Unwana Wave Marketing -<span class="text-slate-900"> Where Marketing Meets Purpose</span></h2>
        <p class="sub-text">
          At Unwana Marketing, we are a team of passionate individuals who thrive on connecting with people, building
          relationships, and driving success in a dynamic and diverse work environment.
        </p>

        <button class="btnMain mr-6" @click="appForm">Careers</button>
        <button class="btnOutline" @click="goTo">About us</button>

        <span class="block cursor-pointer text-sm font-medium text-gray-600" @click="scrollTo"
          >Scroll down to explore</span
        >
      </div>
      <!-- right div -->
      <div>
        <img src="/assets/img/hero.jpg" alt="" />
      </div>
    </div>
  </section>

  <!-- carousel component -->
  <Carousel class="mt-36" />

  <!-- cta section -->
  <Cta>
    <section class="mt-36 flex text-center">
      <div class="bg-gray-100 py-12 border rounded-md h-full">
        <div class="md:w-1/2 mx-auto space-y-8">
          <h2 class="titleText">Welcome to Unwana Media Marketing</h2>
          <p class="sub-text">
            As a company, we are committed to making a positive impact on the non-profit landscape throughout North
            America. We firmly believe that our results-oriented approach sets us apart and empowers our clients to
            achieve remarkable growth.
          </p>
          <div class="space-x-6">
            <button class="btnMain" @click="handleClick">Contact us</button>
            <button class="btnOutline" @click="handleClick">Learn more</button>
          </div>
        </div>
      </div>
    </section>
  </Cta>
</template>
