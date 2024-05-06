<template>
  <div class="main-container">
    <header>
      <div class="banner">
        SIBiLS
      </div>
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/biodiversitypmc">BiodiversityPMC</RouterLink>
        <RouterLink to="/variomes">Variomes</RouterLink>
      </nav>
    </header>
    <RouterView />
  </div>
</template>

<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<style scoped>

.main-container {
  display: flex;
  flex-direction: column;
  width: 100%;
}

header {
  line-height: 1.5;
  max-height: 100vh;
  width: 100%;
}

.banner {
  text-align: center;
  font-size: 1.5rem;
  padding: 1rem 0;
  background: #CC0000;
  color: #ffffff;
  width: 100%
}

nav {
  text-align: center;
  font-size: 12px;
  padding: 1rem 0;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}


</style>
