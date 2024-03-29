<script setup></script>

<template>
  <!-- hero section -->
  <section class="h-screen-[5rem]">
    <div class="grid grid-cols-1 md:grid-cols-2 h-full items-center gap-10">
      <!-- left div -->
      <div class="space-y-6">
        <h2 class="lead">How can we help? ></h2>
        <p class="sub-text">
          Let us help by answering any questions you may have
        </p>

        <button class="btnMain mr-6" @click="appForm">Careers</button>
        <button class="btnOutline" @click="goTo">About us</button>

        <span
          class="block cursor-pointer text-sm font-medium text-gray-600"
          @click="scrollTo"
          >Scroll down to explore</span
        >
      </div>
      <!-- right div -->
      <div>
        <img src="/assets/img/contact.jpg" alt="" />
      </div>
    </div>
  </section>

  <!-- contact form -->
  <section class="mt-32">
    <div class="text-center space-y-4 w-1/2 mx-auto">
      <h2 class="subLead">Send us a message</h2>
      <p class="sub-text">
        Let us help you with any questions you may have. We are here to help you
        grow your business
      </p>
    </div>

    <form class="space-y-8 mt-20" @submit.prevent>
      <BaseInput label="Full name" type="text" required />
      <BaseInput label="Email" type="email" required />
      <BaseInput label="Subject" type="text" />
      <div class="space-y-2 mt-2 text-start">
        <Label>Your message</Label>
        <TextMsg />
      </div>

      <button class="btnMain">Send message</button>
    </form>
  </section>

  <!-- join us section -->
  <section class="mt-36 text-center grid items-center">
    <div class="space-y-4 text-center max-w-[50%] mx-auto">
      <h2 class="titleText">Our Location</h2>
      <p class="sub-text">
        If you are nearby, feel free to drop by our office at any time. We are
        always looking for new talent to join our team!
      </p>

      <!-- location -->
      <div>
        <div class="space-y-4 text-center">
          <!-- icon -->
          <span></span>
          <!-- title -->
          <h3 class="subLead">Lagos</h3>
          <p class="sub-text w-1/2 mx-auto text-center">
            Suite 529 21 Afolabi Obe Street Ijesha, Surulere, Lagos, 5th Floor
            Oasis Building
          </p>
          <p class="sub-text">365-888-4760</p>
          <p class="sub-text">admin@unwana.ca</p>
        </div>
      </div>
    </div>
  </section>

  <!-- cta section -->
  <Cta>
    <section class="mt-36 flex text-center">
      <div class="bg-gray-100 py-12 border rounded-md h-full">
        <div class="w-1/2 mx-auto space-y-8">
          <h2 class="titleText">Our Mission</h2>
          <p class="sub-text">
            Our mission is propelling organizations towards unparalleled
            success. We are dedicated to serving the non-profit sector by
            designing and executing direct marketing campaigns that deliver
            exceptional results. Our focus extends to enhancing customer service
            and sales techniques, as well as driving donor and customer
            acquisition to levels beyond expectations.
          </p>
          <div class="space-x-6">
            <button class="btnMain">Join us today</button>
          </div>
        </div>
      </div>
    </section></Cta
  >
</template>

<style></style>
