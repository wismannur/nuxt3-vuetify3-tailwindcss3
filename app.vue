<template>
  <div id="home">
    <h1 class="text-3xl font-bold underline text-teal-500">Hello world! {{ runtimeConfig.public.projectEnv }}</h1>
  </div>
</template>

<script setup lang="ts">
const runtimeConfig = useRuntimeConfig();

console.log('runtimeConfig ', runtimeConfig)
console.log(`runtimeConfig.public.projectEnv ${runtimeConfig.public.projectEnv}`);
console.log(`runtimeConfig.public.hostAPI ${runtimeConfig.public.hostAPI}`);
</script>
