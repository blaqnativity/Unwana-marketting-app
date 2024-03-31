<script setup>
useHead({
  title: 'Unwana',
})
const router = useRouter()

const gotToCareers = () => {
  router.push({ path: '/Careers/Application' })
}
const gotoAbout = () => {
  router.push({ path: '/About' })
}

const services = [
  {
    name: 'Full-time permanent and part-time positions',
  },
  {
    name: 'Ongoing, in-depth business development training',
  },
  {
    name: 'Merit-based career advancement',
  },
  {
    name: 'Weekly pay',
  },
  {
    name: 'Guaranteed base wages',
  },
  {
    name: 'Uncapped bonus structure',
  },
  {
    name: 'Daily cash bonuses',
  },
  {
    name: 'Opportunities to travel across North America',
  },
  {
    name: 'All-expenses paid team nights!',
  },
]
const qualities = [
  {
    name: 'Works well in a team environment',
  },
  {
    name: 'Disciplined/Responsible',
  },
  {
    name: 'Strong work ethic',
  },
  {
    name: 'Self-motivated',
  },
  {
    name: 'Open Minded',
  },
  {
    name: 'Good people skills',
  },
  {
    name: 'Coachable',
  },
  {
    name: 'Confident',
  },
  {
    name: 'Have Growth Mindset',
  },
]
</script>

<template>
  <!-- hero section -->
  <section class="h-screen-[5rem]">
    <div class="grid grid-cols-1 md:grid-cols-2 h-full items-center gap-10">
      <!-- left div -->
      <div class="space-y-6">
        <h2 class="lead">Join our team today</h2>
        <p class="sub-text">
          Join us at Unwana Marketing, where you'll have the opportunity to work with inspiring colleagues, grow both
          personally and professionally, and be part of a purpose-driven organization that's making waves in the
          marketing industry and beyond. Together, let's make a lasting impact and build a brighter future.
        </p>

        <button class="btnMain mr-6" @click="gotToCareers">Apply now</button>
        <button class="btnOutline" @click="gotoAbout">About us</button>
      </div>
      <!-- right div -->
      <div>
        <img src="/assets/img/time.jpg" alt="" />
      </div>
    </div>
  </section>

  <!-- what we offer -->
  <section class="mt-36 text-center grid items-center">
    <div class="space-y-10 text-center md:max-w-[50%] mx-auto">
      <h2 class="titleText">What We Offer</h2>
      <p class="sub-text">
        We emphasize the development and growth of our team members. That means near limitless earning potential,
        competitive wages, a generous bonus structure, and ample opportunities to build connections with our growing
        network of business partners.
      </p>

      <!-- services list -->
      <ul class="grid grid-cols-1 gap-4">
        <li v-for="service in services" :key="service" class="flex items-center gap-4 sub-text">
          <img src="/assets/img/checkicon.png" alt="" class="w-6 h-auto" />
          {{ service.name }}
        </li>
      </ul>
    </div>
  </section>
  <!-- Our Qualities -->
  <section class="mt-20 text-center grid items-center">
    <div class="space-y-10 text-center md:max-w-[50%] mx-auto">
      <h2 class="titleText">Qualities</h2>
      <p class="sub-text">
        Prior fundraising experience is an asset! However, no prior fundraising/marketing experience is necessary, as
        all training is completed in house!
      </p>

      <!-- services list -->
      <ul class="grid grid-cols-1 gap-4">
        <li v-for="quality in qualities" :key="quality" class="flex items-center gap-4 sub-text">
          <img src="/assets/img/checkicon.png" alt="" class="w-6 h-auto" />
          {{ quality.name }}
        </li>
      </ul>
    </div>
  </section>

  <!-- our mission cta section -->
  <Cta>
    <section class="mt-36 flex text-center">
      <div class="bg-gray-100 py-12 border rounded-md h-full">
        <div class="md:w-1/2 mx-auto space-y-8">
          <h2 class="titleText">Our Mission</h2>
          <p class="sub-text">
            Our mission is propelling organizations towards unparalleled success. We are dedicated to serving the
            non-profit sector by designing and executing direct marketing campaigns that deliver exceptional results.
            Our focus extends to enhancing customer service and sales techniques, as well as driving donor and customer
            acquisition to levels beyond expectations.
          </p>
          <div class="space-x-6">
            <button class="btnMain">Join us</button>
          </div>
        </div>
      </div>
    </section></Cta
  >
</template>
