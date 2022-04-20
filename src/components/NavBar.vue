<template>
  <div class="nav">
    <div class="logo">
      <img src="../assets/logo.svg" alt="mars logo" class="logo" />
    </div>
    <div class="nav-link">
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/">About</RouterLink>
      <RouterLink to="/">Portfolio</RouterLink>
      <RouterLink to="/">Contact</RouterLink>
    </div>
    <RouterView />
  </div>
</template>
<script>
import { RouterLink, RouterView } from "vue-router";
export default {
  component: {
    RouterLink,
    RouterView,
  },
};
</script>
<style>
@import "../style/NavBar.css";
</style>
