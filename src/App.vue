<script setup>
import AppHeader from './components/AppHeader.vue'
import AppFooter from './components/AppFooter.vue'
</script>

<template>
  <AppHeader title="My Site" />

  <main>
    <section id="home">
      <h1>Welcome!</h1>
      <p>This is the home section.</p>
    </section>

    <section id="about">
      <h2>About</h2>
      <p>This is the about section.</p>
    </section>

    <section id="contact">
      <h2>Contact</h2>
      <p>This is the contact section.</p>
    </section>
  </main>

  <AppFooter />
</template>

<style>
body { margin: 0; }
section { padding: 2rem; }

@media (max-width: 600px) {
  section { padding: 1rem; }
  h1 { font-size: 1.75rem; }
}
</style>