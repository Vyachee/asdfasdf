<template>
  <div class="container">
    <p style="color: white">
      {{ $store.state.title }}
      {{ $store.state.auth.login}}
    </p>
    <Input title="Логин" :value="login"/>
    <Input title="Пароль" type="password"  :value="password"/>
    <Button>Войти</Button>
  </div>
</template>

<script setup lang="ts">

import Input from "@/components/Input.vue";
import Button from "@/components/Button.vue";
import {useStore} from "vuex";
import {computed} from "vue";

const store = useStore();

const login = computed(() => store.state.auth.login)
const password = computed(() => store.state.auth.password)
</script>

<style scoped lang="scss">
.container {
  max-width: 315px;
  display: flex;
  flex-direction: column;
  align-items: stretch;
  gap: 10px;
}
</style>
