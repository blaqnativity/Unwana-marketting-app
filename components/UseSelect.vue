<script setup>
const props = defineProps({
  label: {
    type: String,
    default: '',
  },
  selectedOpt: {
    type: String,
    default: '',
  },
  options: {
    type: Array,
    required: true,
  },
})

const selectedOpt = ref(null)

const toggleOpt = (option) => {
  selectedOpt.value = option
}
</script>

<template>
  <div class="grid space-y-4 text-start relative">
    <label v-if="label">{{ label }}</label>
    <div
      class="dropdown-wrapper rounded-md py-2 font-bold text-gray-500 cursor-pointer flex justify-between px-2 items-center border-[2px]"
    >
      <p>{{ selectedOpt || 'Select your option' }}</p>
      <img src="/assets/img/down.svg" class="w-8 h-auto" />
    </div>
    <div
      class="optionVisible absolute bg-white space-y-4 gb-gray-200 shadow-lg shadow-gray-400 rounded-lg w-full top-[5rem] border"
    >
      <div
        class="hidden flex justify-between w-full px-4 py-2 cursor-pointer"
        v-for="(option, index) in options"
        :key="index"
        @click="toggleOpt(option)"
      >
        <p class="text-gray-500 font-bold">{{ option }}</p>
      </div>
    </div>
  </div>
</template>

<style></style>
