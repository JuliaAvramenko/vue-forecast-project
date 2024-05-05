<script setup>
defineProps({
  modelValue: {
    type: String,
  }
});
  
defineEmits(['update:modelValue']);
</script>

<template>
    <div>world {{ modelValue }}</div>
    <button
    @click="$emit('update:modelValue', 'test2')">Изменить в parent</button>
</template>
<script>
</script>
<style></style>