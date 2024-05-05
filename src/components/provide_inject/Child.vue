<script setup>
import { inject} from 'vue';
  
  const { value, changeValue } = inject('value');
</script>

<template>
    <div>{{ value }}world</div>
    <button @click="changeValue('test child')">Изменить в parent</button>
</template>
<script>
</script>
<style></style>