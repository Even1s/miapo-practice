<template>
  <div class="counter">
    <h1>This is an counter page</h1>
    <button @click.prevent="increment()">+</button>
    <p>Your counter: {{ count }}</p>
    <p>Double counter: {{ doubleCount }}</p>
  </div>
</template>

<script setup lang="ts">
import { useCounterStore } from '@/stores/counter.ts'
import { storeToRefs } from 'pinia'

const { count, doubleCount } = storeToRefs(useCounterStore());
const { increment } = useCounterStore();
</script>

<style>
@media (min-width: 1024px) {
  .counter {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 16px;
  }
}
</style>
