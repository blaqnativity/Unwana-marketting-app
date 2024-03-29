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
      type="type"
      v-bind="$attrs"
      @input="$emit('update:modelValue', evetnt.target.value)"
    />
  </div>
</template>
