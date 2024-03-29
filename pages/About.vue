<script setup>
const router = useRouter();
useHead({
  title: "Uwana",
});

const gotToCareers = () => {
  router.push({ path: "/Careers/Application" });
};
const gotoContact = () => {
  router.push({ path: "/Contact" });
};
</script>

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

        <div class="space-x-6">
          <button class="btnMain" @click="gotoContact">Contact us</button>
          <button class="btnOutline" @click="gotToCareers">Careers</button>
        </div>
      </div>
      <!-- right div -->
      <div>
        <img src="/assets/img/time.jpg" alt="" />
      </div>
    </div>
  </section>

  <!--  -->
  <section class="h-screen-[5rem] mt-20">
    <div class="mb-14">
      <h2 class="lead">Learn more</h2>
      <p class="sub-text">Here is a little bit more about who we are</p>
    </div>
    <div class="grid grid-cols-1 md:grid-cols-2 h-full items-center gap-10">
      <!-- left div -->
      <div>
        <img src="/assets/img/team.jpg" alt="" />
      </div>
      <!-- right div -->
      <div class="space-y-6">
        <p class="sub-text">
          For the past decade, our company has been a dedicated partner in
          helping businesses and organizations achieve their objectives and
          reach their revenue goals. As a dynamic marketing and fundraising
          firm, we are committed to empowering our clients' brands and driving
          their success through our comprehensive services. Our expertise lies
          in designing and executing impactful direct marketing campaigns that
          resonate with the target audience and drive tangible results As an
          emerging player in the marketing industry, we firmly believe in the
          power of investing in our people. We are committed to your personal
          and professional growth, providing ample opportunities for learning,
          skill development, and advancement. Whether it's through regular team
          meetings, mentorship programs, or access to industry-leading training,
          we are dedicated to helping you reach new heights in your career.
          Beyond our work, we are proud to be actively engaged in community
          service and social impact initiatives. Unwana Marketing is more than
          just a company; we are a force for good, driven by the belief that we
          can create a positive change in the lives of others.
        </p>
      </div>
    </div>
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
      <div class="grid md:grid-cols-2 gap-4">
        <div class="space-y-4 text-start">
          <!-- icon -->
          <span></span>
          <!-- title -->
          <h3 class="subLead">Lagos</h3>
          <p class="sub-text">
            Suite 529 21 King Street West, 5th Floor Hamilton Ontario L8P 4W7
          </p>
          <p class="sub-text">365-888-4760</p>
          <p class="sub-text">admin@unwana.ca</p>
        </div>
        <!-- map -->
        <div></div>
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
            <button class="btnMain">Join us</button>
          </div>
        </div>
      </div>
    </section></Cta
  >
</template>
