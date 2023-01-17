<template>
  <div id="home">
    <h1 class="text-3xl font-bold underline text-teal-500">Hello world! {{ runtimeConfig.public.lmsEnv }}</h1>
  </div>
</template>

<script setup lang="ts">
const runtimeConfig = useRuntimeConfig();

console.log(runtimeConfig.apiSecret);
console.log(runtimeConfig.public.apiBase);
console.log(runtimeConfig.public.lmsEnv);
</script>
