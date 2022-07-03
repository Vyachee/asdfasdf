<template>
  <div>
    <slot/>
  </div>
</template>

<script setup lang="ts">
  defineProps({
    title: String
  })
</script>

<style scoped lang="scss">
  div {
    background-color: #FAD200;
    border-radius: 10px;
    color: #000;
    padding: 10px;
    font-weight: 700;
    font-size: 15px;
    cursor: pointer;
    text-align: center;
  }
</style>
