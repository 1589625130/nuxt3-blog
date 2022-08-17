<template>
  <div>
    <NuxtWelcome/>
  </div>
</template>

<script setup>
import {ref} from "vue";

const route = useRoute();


console.log('search-info.vue', route.params)
</script>

<style scoped>

</style>
