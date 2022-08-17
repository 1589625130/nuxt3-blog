<template>
  <nuxt-layout name="main">
    <template #left>
      <div>
        <h1>left</h1>
        <div>
          <nuxt-link to="/about">about</nuxt-link>
        </div>
        <el-button type="primary">click</el-button>
        <!--        <div>{{ list }}</div>-->
      </div>


    </template>

    <template #right>
      <h1>right</h1>

    </template>

  </nuxt-layout>
</template>

<script setup>
import {ref} from 'vue'
import {ElButton} from 'element-plus'

console.log('index.vue')
const {data, error, pending, refresh} = await useAsyncData("getList", () =>
    $fetch("http://121.36.81.61:8000/getTenArticleList")
);

const res = await useFetch("http://121.36.81.61:8000/getTenArticleList");
console.log({res})
const list = ref(res.data._rawValue.data);
console.log({data, error, pending, refresh});
</script>

<style scoped>

</style>
