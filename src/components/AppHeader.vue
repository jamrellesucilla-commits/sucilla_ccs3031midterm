<script setup>
defineProps({ title: String })
</script>

<template>
  <header class="header">
    <h2>{{ title }}</h2>
    <nav>
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>
</template>

<style scoped>
.header {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  background: #2c3e50;
  color: white;
}
nav { display: flex; gap: 1rem; }
nav a { color: white; text-decoration: none; }

@media (max-width: 600px) {
  .header {
    flex-direction: column;
    gap: 0.5rem;
    padding: 1rem;
  }
}
</style>