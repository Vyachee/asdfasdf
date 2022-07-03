<template>
  <div class="wrap">
    <LoginWindow/>
  </div>
</template>

<script lang="ts" setup>
import Input from "@/components/Input.vue";
import Button from "@/components/Button.vue";
import LoginWindow from "@/components/LoginWindow.vue";
</script>

<style lang="scss">

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

#app {
  font-family: 'Montserrat', sans-serif;
}

.wrap {
  background-color: #212121;
  width: 100vw;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

</style>
