<script setup lang="ts">
  import type { Css } from 'tide-package-library-poc';
  import { CSS, TideButton } from 'tide-package-library-poc';

  const test: Css = CSS.BG_YELLOW;

  console.log('const:', CSS);
  // console.log('type:', Css);
</script>

<template>
  <h1 :class="[CSS.MB_1]">TIDE Consumer App Demo</h1>
  <TideButton :class="[CSS.MB_1]">Consumer</TideButton>
  <TideButton :is-red="true">Consumer</TideButton>
</template>

<style scoped>
</style>
