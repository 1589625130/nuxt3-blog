<template>
  <div>
    <h1>about</h1>
    <nuxt-link to="/">首页</nuxt-link>
    <lazyText v-show="show"/>
    <button @click="clickShow">点击</button>
  </div>
</template>

<script setup>
import {ref} from 'vue'

const show = ref(false)

function clickShow() {
  show.value = true
}

</script>

<style scoped>

</style>
