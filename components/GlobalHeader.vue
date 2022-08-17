<template>
  <div class="header">
    <el-menu mode="horizontal"
             :default-active="state.activeIndex"
             class="el-menu-demo"
             background-color="#545c64"
             text-color="#fff"
             active-text-color="#ffd04b"
             @select="selectMenu"
    >
      <el-menu-item v-for="(item,index) of menuList" :index="index" :key="index">{{ item.name }}</el-menu-item>
    </el-menu>
  </div>
</template>

<script setup>
import { ElMenu, ElMenuItem } from "element-plus";
import { useRoute, useState } from "nuxt/app";

const menuList = [
  {
    path: "/",
    name: "首页"
  },
  {
    path: "/about",
    name: "关于"
  },
  {
    path: "/contact",
    name: "联系"
  }
];

const state = useState("menu", () => {
  return { activeIndex: "" };
});

const route = useRoute();
const routeObj = {
  index: 0,
  about: 1
};
state.activeIndex = routeObj[route.name];
console.log({ state: state.activeIndex });

function selectMenu(index) {
  state.activeIndex = index;
  navigateTo(menuList[index].path);
}

</script>

<style scoped>

</style>
