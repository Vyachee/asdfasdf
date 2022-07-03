<template>
  <div>
    <span>{{title}}</span>
    <input :type=type v-bind="$store.state.auth.login" v-once :placeholder=title>
  </div>
</template>

<script setup lang="ts">
  defineProps({
    title: String,
    type: {
      type: String,
      default: 'text'
    },
    value: String
  })
</script>

<style scoped lang="scss">
  div {
    background-color: #171717;
    border-radius: 10px;
    padding: 15px;
    display: flex;
    flex-direction: column;
    align-items: start;
    font-family: 'Montserrat', sans-serif;
    input {
      background-color: transparent;
      border: none;
      outline: none;
      color: #fff;
      font-size: 20px;
      font-weight: 700;
      margin-top: 5px;
      &::placeholder {
        color: #D6D6D6;
      }
    }
    span {
      font-weight: 500;
      color: #D6D6D6;
    }
  }
</style>
