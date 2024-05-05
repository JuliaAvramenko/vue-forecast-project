<script setup>
import { provide, ref } from 'vue';
import Child from './Child.vue';

const value = ref('blabla')

const changeValue = (a) =>{
    value.value = a
}

provide('value', {
  value,
  changeValue,
});
</script>

<template>
    <div>{{value}}Hello</div>
    <Child></Child>
    <button @click="changeValue('test parent')">
      Изменить
    </button>
</template>
<script></script>
<style></style>
