<script setup lang="ts">
  import type { Css } from 'tide-package-library-poc/types/Css';

  import TideButton from 'tide-package-library-poc/components/TideButton';
  import { CSS } from 'tide-package-library-poc/types/Css';
  import { sayGoodbye, sayHello } from 'tide-package-library-poc/utilities/say';

  import 'tide-package-library-poc/styles';

  import BasicButton from '@/components/BasicButton.vue';

  const test: Css = CSS.BG_YELLOW;

  console.log('TEST:', test);

  sayHello();
  sayGoodbye();
</script>

<template>
  <h1 :class="[CSS.MB_1]">TIDE Consumer App Demo</h1>
  <BasicButton :class="[CSS.MB_1]">Test 1</BasicButton>
  <TideButton :class="[CSS.MB_1]" :id="2">Test</TideButton>
  <TideButton :class="[CSS.MB_1]" :id="3" :is-large="true">Test</TideButton>
</template>

<style scoped>
</style>
