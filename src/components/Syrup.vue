<template>
    <div v-if="currentSyrup.id !== 's1'" class="syrup" :style="{ background:
  `repeating-linear-gradient(45deg, white, white 10px, ${currentSyrup.color}
  10px, ${currentSyrup.color} 20px)` }"></div>
  </template>

<!-- <div class="baseBeverage" :style="{ backgroundColor: currentBase.color }">
  </div>-->

<script setup lang="ts">
    import { currentSyrup } from "../stores/beverage";
</script>
<style lang="scss" scoped>
.syrup {
  transform: translateY(400%);
  background-color: #c6c6c6;
  position: relative;
  width: 100%;
  height: 20%;
  animation: pour-tea 2s 1s forwards;
  z-index: 2;
}
</style>
