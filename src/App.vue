<script setup>
import { ref, onMounted } from 'vue';

let count = ref(0);
let title = 'Hello Vue';

onMounted(() => {
  console.log('mounted');
});

const increseCount = () => {
  count.value++;
};
</script>

<template>
  <h1>{{ title }}</h1>
  <button @click="increseCount">count++</button>
  <p>{{ count }}</p>
</template>

<style scoped></style>
