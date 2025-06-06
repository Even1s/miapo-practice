<template>
  <div class="about">
    <h1>This is an about page</h1>
    <p>We are working on projects for Serious Companies</p>
    <p><b>Only Serious!!</b></p>
  </div>
</template>

<script setup lang="ts">
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
