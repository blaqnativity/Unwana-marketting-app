<script setup>
const error = useError();
defineProps({
  label: String,
  modelValue: String,
});
</script>

<template>
  <div>
    <textarea rows="2" :value="modelValue" v-bind="$attrs"></textarea>
  </div>
</template>
