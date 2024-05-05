<script setup>
import { ref } from 'vue';
import Child from './Child.vue';

const value = ref('blabla')

const changeValue =(a) =>{
    value.value = a || 'test'
}
</script>

<template>
    <div>Hello</div>
    <Child v-model="value"></Child>
    <button @click="changeValue">
      Изменить
    </button>
</template>
<script></script>
<style></style>
