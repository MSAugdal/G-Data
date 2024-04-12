<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <main>
    <div class="wrapper">
      <p class="header">GåData</p>
      <p class="text">La hvert skritt telle</p>
      <RouterLink to="/login" class="mybutton"><button>Lær mer</button></RouterLink>
    </div>
  </main>
</template>

<style scoped>
main {
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
}
.wrapper p.header {
  font-size: 5rem;
  margin: -1rem;
  padding: 0;
  font-weight: 400;
}
.wrapper .text {
  font-size: 3rem;
  margin: 0;
  padding: 0;
  color: hsla(185, 75%, 94%, 64%);
  font-weight: 300;
}
button {
  transition: 0.5s;
  /* background-color: var(--primary-500); */
  background-color: transparent;
  margin-top: 2rem;
  border: 2px solid var(--primary-700);
  border-radius: 8px;
  width: 240px;
  height: 48px;

  color: var(--text-50);
  font-size: 1rem;
  font-weight: 600;
}
button:hover {
  transition: 0.25s;
  transform: scale(1.08);
  color: var(--text-200);
  border: 2px solid var(--background-200);
  background-color: var(--background-900);
}
.mybutton {
  text-decoration: none;
  background-color: transparent;
}
</style>
