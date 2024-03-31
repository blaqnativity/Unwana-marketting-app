<script setup>
const router = useRouter()
useHead({
  title: 'Uwana',
})

const gotoContact = () => {
  router.push({ path: '/Contact' })
}
const gotoCareers = () => {
  router.push({ path: '/careers/application' })
}
</script>

<template>
  <!-- hero section -->
  <section class="h-screen-[5rem]">
    <div class="grid grid-cols-1 md:grid-cols-2 h-full items-center gap-10">
      <!-- left div -->
      <div class="space-y-6">
        <h2 class="lead">Elevate Impact through Strategic Engagement</h2>
        <p class="sub-text">
          Empowering Non-Profits and Businesses to Forge Lasting Connections, Drive Sales, and Achieve Remarkable Growth
        </p>
        <div class="space-x-6">
          <button class="btnMain" @click="gotoContact">Contact us</button>
          <button class="btnOutline" @click="gotoCareers">Careers</button>
        </div>

        <span class="block cursor-pointer text-sm font-medium text-gray-600" @click="scrollTo"
          >Scroll down to explore</span
        >
      </div>
      <!-- right div -->
      <div>
        <img src="/assets/img/marketting.jpg" alt="" />
      </div>
    </div>
  </section>

  <!-- join us section -->
  <section class="mt-36">
    <div class="grid cols-1 items-center max-w-[80%] mx-auto">
      <div class="space-y-4 text-center">
        <h2 class="titleText">Welcome to Unwana Marketing</h2>
        <p class="sub-text">Here are the services offered by Unwana</p>
      </div>

      <!-- grid items -->
      <div class="my-10 grid md:grid-cols-2 items-start gap-4">
        <!-- img div -->
        <img src="/assets/img/customercare.jpg" class="h-[400px]" />
        <!-- content div -->
        <div class="flex flex-col space-y-6">
          <!-- icon -->
          <span></span>
          <!-- title -->
          <h2 class="subLead">Sales & Customer Service</h2>
          <!-- paragragh text -->
          <p class="sub-text">
            As the first point of contact, these teams are instrumental in establishing and maintaining positive
            relationships with customers, driving sales, and ensuring a high level of customer satisfaction. At Unwana
            Marketing, we understand the significance of these pivotal roles, and that's why we invest in training and
            building dedicated teams that are passionate about protecting brand integrity. By equipping our teams with
            the necessary skills and resources, we empower them to provide exceptional service and deliver on our
            promise of professionalism.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>
