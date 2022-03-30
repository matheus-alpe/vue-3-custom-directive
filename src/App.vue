<template>
  <h1>Without directive</h1>
  <h1 v-font-size>With 'font-size' directive</h1>
  <h1 v-font-size.small>With 'font-size' directive modifier:small</h1>
  <h1 v-font-size.large>With 'font-size' directive modifier:large</h1>
  <h1 v-font-size="fontSize">With 'font-size' directive value</h1>
  <h1 v-font-size.red="fontSize">With 'font-size' directive value and modifier: red</h1>

  <button @click="fontSize *= 2">Multiply font-size</button>
</template>

<script setup>
import { ref } from 'vue'

const fontSize = ref(11)
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
