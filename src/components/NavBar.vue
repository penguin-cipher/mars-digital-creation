<template>
  <div class="nav">
    <div class="logo">
      <img src="../assets/logo.svg" alt="mars logo" class="logo" />
    </div>
    <div
      class="ham-menu"
      @click="changeVisibility()"
      :class="{ active: burgerVisibility }"
    >
      <span class="menue-bar"></span>
      <span class="menue-bar"></span>
      <span class="menue-bar"></span>
    </div>
    <nav class="nav-wrap" :class="{ open: burgerVisibility }">
      <ul class="nav-list" @click="burgerVisibility = false">
        <RouterLink to="/" class="nav-link">Home</RouterLink>
        <RouterLink to="/about" class="nav-link">About</RouterLink>
        <RouterLink to="/portfolio" class="nav-link">Portfolio</RouterLink>
        <RouterLink to="/contact" class="nav-link">Contact</RouterLink>
      </ul>
    </nav>
  </div>
</template>
<script>
import { RouterLink, RouterView } from "vue-router";
export default {
  component: {
    RouterLink,
    RouterView,
  },
  data() {
    return {
      burgerVisibility: false,
    };
  },
  methods: {
    changeVisibility() {
      this.burgerVisibility = !this.burgerVisibility;
    },
  },
};
</script>
<style>
@import "../style/NavBar.css";
</style>
