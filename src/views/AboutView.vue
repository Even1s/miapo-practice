<template>
  <div class="about">
    <h1>This is an about page</h1>
    <input v-model="value">
    <p>Your value: {{ value }}</p>
  </div>
</template>

<script setup lang="ts">
import {ref} from "vue";

const value = ref<string>('');
</script>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 16px;
  }
}
</style>
