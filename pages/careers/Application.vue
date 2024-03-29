<script setup>
const router = useRouter();
useHead({
  title: "Uwana",
});

const handleClick = () => {
  router.push({ path: "/About" });
  // navigateTo("/About");
};
</script>

<template>
  <!-- Application form -->
  <section class="mt-10">
    <div class="text-center space-y-4">
      <div>
        <h2 class="lead">Application</h2>
        <p class="sub-text">
          Please fill out each step in the application form below
        </p>
      </div>

      <!-- form -->
    </div>
  </section>
  <!-- hero section -->
</template>
