<script setup>
defineProps({
  label: String,
  modelValue: String,
});
</script>

<template>
  <div>
    <label v-if="label">{{ label }}</label>
    <textarea
      type="type"
      v-bind="$attrs"
      @input="$emit('update:modelValue', evetnt.target.value)"
    />
  </div>
</template>
