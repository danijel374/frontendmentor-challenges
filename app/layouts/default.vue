<script lang="ts" setup>
  const { loggedIn, user, clear } = useUserSession();
</script>

<template>
  <nav class="container mx-auto">
    My navigation here
    <UButton
      v-if="!loggedIn"
      to="/api/auth/github"
      icon="i-simple-icons-github"
      label="Login with GitHub"
      size="xs"
      external
    />
  </nav>
  <slot />
</template>

<style></style>
