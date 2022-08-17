<template>
  <div>
    <h1>{{ id }}</h1>
    
  </div>
</template>

<script setup>
import {ref} from "vue";

const route = useRoute();
const id = ref(route.params.id);

console.log('home.vue', id.value)
</script>

<style scoped>

</style>
