<script lang="ts" setup>
  const { loggedIn, user, clear } = useUserSession();
  const exampleProject = {
    name: "",
    difficulty: "newbie",
    languages: ["html", "css"],
  };
</script>

<template>
  <main class="container mx-auto">
    <h1 class="text-2xl">Projects bellow here!</h1>
    <ul>
      <UButton
        v-if="!loggedIn"
        to="/api/auth/github"
        icon="i-simple-icons-github"
        label="Login with GitHub"
        size="xs"
        external
      />
    </ul>

    <form action="">
      <input type="text" />
      <button>Add a project here</button>
    </form>
  </main>
</template>

<style></style>
