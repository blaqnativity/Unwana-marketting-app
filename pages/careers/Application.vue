<script setup>
definePageMeta({
  layout: 'custom',
  title: 'Unwana markettin',
}),
  useHead({
    title: 'Unwana',
  })

const options = ref(['Yes', 'No'])
const options2 = ref(['Full time 40 hrs per week', 'Per time 30 hrs per week approx'])
</script>

<template>
  <!-- Application form -->
  <section class="mt-10">
    <div class="text-center space-y-4">
      <div>
        <h2 class="lead">Application</h2>
        <p class="sub-text">This information will be displayed publicly so be careful what you share</p>
      </div>

      <form @submit.prevent class="space-y-14">
        <div class="space-y-12">
          <!-- Personal bio-data -->
          <div class="border-b border-gray-900/10 pb-12">
            <h2 class="text-base font-semibold leading-7 text-gray-900">Personal Information</h2>

            <div class="mt-10 grid grid-cols-1 gap-x-6 gap-y-8">
              <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                <BaseInput label="First name" />
                <BaseInput label="Last name" />
              </div>

              <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                <BaseInput label="Email" />
                <BaseInput label="Phone" />
              </div>
            </div>
          </div>

          <!-- upload Resume -->
          <div class="border-b border-gray-900/10 pb-12">
            <h2 class="text-base font-semibold leading-7 text-gray-900">Resume</h2>
            <div class="border-b border-gray-900/10 pb-12">
              <div class="mt-10 grid grid-cols-1 gap-x-6 gap-y-8 sm:grid-cols-6">
                <div class="col-span-full">
                  <label for="cover-photo" class="block text-sm font-medium leading-6 text-gray-900"
                    >Upload resume</label
                  >
                  <div class="mt-2 flex justify-center rounded-lg border border-dashed border-gray-900/25 px-6 py-10">
                    <div class="text-center">
                      <img src="/assets/img/cloud.svg" class="w-12 h-auto mx-auto" />
                      <div class="mt-4 flex text-sm leading-6 text-gray-600">
                        <label
                          for="file-upload"
                          class="relative cursor-pointer rounded-md bg-white font-semibold text-indigo-600 focus-within:outline-none focus-within:ring-2 focus-within:ring-indigo-600 focus-within:ring-offset-2 hover:text-indigo-500"
                        >
                          <span>Select file</span>
                          <input id="file-upload" name="file-upload" type="file" class="sr-only" />
                        </label>
                        <p class="pl-1">or drag and drop</p>
                      </div>
                      <p class="text-xs leading-5 text-gray-600">PDF / WORD file up to 10MB</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <!-- select dropdown -->
          <div class="space-y-6">
            <UseSelect label="Are you willing to be on your feet for at least 5 hrs per day? *" :options="options" />

            <UseSelect label="Position Preference  *" :options="options2" />
            <UseSelect
              label="Do you have any pervious experience working with Charities or Non Profit Organizations?"
              :options="options"
            />
            <UseSelect label="Is English your first or primary language" :options="options" />
          </div>

          <div class="flex items-center justify-end gap-x-6">
            <button class="btnOutline">Cancel</button>
            <button class="btnMain">Save</button>
          </div>
        </div>

        <!-- date selector -->
        <div class="space-y-6">
          <Date-picker />
        </div>
      </form>
    </div>
  </section>
  <!-- hero section -->
</template>
