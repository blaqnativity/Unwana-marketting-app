<script setup>
defineProps({
  label: String,
  modelValue: String,
});
</script>

<template>
  <div class="items-start flex flex-col space-y-2">
    <label v-if="label">{{ label }}</label>
    <input
      :value="modelValue"
      v-bind="$attrs"
      @input="$emit('update:modelValue', event.target.value)"
    />
  </div>
</template>
