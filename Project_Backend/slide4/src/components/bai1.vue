<template>
  <div>
    <h1>Calculator: 04 - Quach Thanh Danh</h1>
    <h3>Count {{ count }}</h3>

    <button @click="increment">+</button>
    <button @click="decrement">-</button>
    <button @click="reset">Reset</button>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)

const increment = () => count.value++
const decrement = () => count.value--
const reset = () => (count.value = 0)
</script>

<style lang="scss" scoped>
button {
  margin: 5px;
  padding: 8px 12px;
}
</style>