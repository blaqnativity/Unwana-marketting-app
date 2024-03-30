<template>
  <div class="sm:col-span-3">
    <label v-if="label">{{ label }}</label>
    <div class="mt-2">
      <select
        v-bind="$attrs"
        :value="modelValue"
        @input="$emit('update:modelValue', $event.target.value)"
      >
        <option
          v-for="option in options"
          :value="option.value"
          :key="option.value"
        >
          {{ option.label }}
        </option>
      </select>
    </div>
  </div>
</template>

<script setup>
const options = ref([]);
const modelValue = ref("");
defineProps({
  label: String,
  options: {
    type: Array,
    default: () => [],
  },
});
</script>
