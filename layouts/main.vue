<template>
  <div class="main">
    <div class="left">
      <slot name="left"></slot>
    </div>
    <div class="right">
      <slot name="right"></slot>
    </div>
  </div>
</template>

<script setup>
console.log('main.vue')
</script>

<style scoped>
.main {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.main .left,
.main .right {
  width: 50%;
  max-height: 700px;
  overflow: auto;
}

.left {
  background-color: darkcyan;
}

.right {
  background-color: antiquewhite;
}
</style>
