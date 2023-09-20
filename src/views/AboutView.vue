<template>
  <div class="about">
    <h1>count:{{ countStore.count }}</h1>
    <button @click="countStore.increment()">+1</button>
  </div>
</template>
<script setup>
import { useCounterStore } from "../stores/counter";
const countStore = useCounterStore();
</script>
<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
