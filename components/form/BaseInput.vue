<script setup>
defineProps({
  modelValue: String,
});
</script>

<template>
  <input
    v-bind="$attrs"
    @input="$emit('update:modelValue', evetnt.target.value)"
  />
</template>
