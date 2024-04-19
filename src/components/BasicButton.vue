<script lang="ts" setup>
</script>

<template>
  <button class="basic-button">
    <span>LOCAL: </span>
    <slot />
  </button>
</template>

<style scoped>
  .basic-button {
    border: 1px solid red;
    border-radius: 0.25rem;
    padding: 0.5rem;
    background-color: pink;
  }
</style>
