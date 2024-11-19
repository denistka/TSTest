<template>
  <div class="display">
    <h2>Display</h2>
    <p>Current value: {{ store.count }}</p>
  </div>
</template>

<script setup>
import { useCounterStore } from '../stores/counter'

const store = useCounterStore()
</script>

<style scoped>
.display {
  padding: 20px;
  text-align: center;
  margin-top: 20px;
  border: 1px solid #ccc;
  border-radius: 8px;
  background-color: #f9f9f9;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

h2 {
  color: #333;
  margin-bottom: 15px;
}

p {
  font-size: 18px;
  color: #666;
}
</style>
