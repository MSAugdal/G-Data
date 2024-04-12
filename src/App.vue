<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template class="wrap_template">
  <header>
    <img src="" alt="GåData©" />
    <div class="wrapper">
      <nav>
        <router-link class="button" to="/">Home</router-link>
        <router-link class="button" to="/dataviz">DataViz</router-link>
        <router-link class="button" to="/faq">FAQ</router-link>
        <router-link class="button" to="/login">Login</router-link>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
@import './assets/base.css';
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
img {
  color: var(--text-200);
}

nav {
    display: flex;
    gap: .5rem;
}
.button {
    transition: .25s;
    padding: .5rem 1rem;
    border-radius: 8px;
    border: 1px solid transparent;
}
.button:hover {
    border: 1px solid var(--background-200);
    background-color: var(--background-900);
}
</style>
