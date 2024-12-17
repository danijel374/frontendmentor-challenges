<script lang="ts" setup>
  definePageMeta({
    middleware: ["auth"],
  });
  const { user } = useUserSession();
</script>

<template>
  <h1>Projects</h1>
  <h2>Welcome {{ user }}</h2>
</template>

<style></style>
