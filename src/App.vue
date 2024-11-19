<script setup>
import Counter from './components/Counter.vue'
import Display from './components/Display.vue'
</script>

<template>
  <header>
    Think Studio Test
  </header>

  <main>
    <Counter />
    <Display />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
  text-align: center;
  padding: 20px;
  font-size: 24px;
  font-weight: bold;
}

main {
  max-width: 600px;
  margin: 0 auto;
  padding: 20px;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }
}
</style>
