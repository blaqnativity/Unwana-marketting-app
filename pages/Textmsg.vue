<script setup>
defineProps({
  modelValue: String,
});
</script>

<template>
  <div>
    <!-- <textarea
      v-bind="$attrs"
      :value="modelValue"
      @input="$emit('update:modelValue', event.target.value)"
      cols="30"
      rows="10"
    ></textarea> -->

    <input type="text" />
  </div>
</template>
