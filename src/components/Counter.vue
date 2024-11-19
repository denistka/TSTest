<template>
  <div class="counter">
    <h2>Counter</h2>
    <div class="buttons">
      <button @click="store.increment()">+</button>
      <span class="count">{{ store.count }}</span>
      <button @click="store.decrement()">-</button>
    </div>
  </div>
</template>

<script setup>
import { useCounterStore } from '../stores/counter'

const store = useCounterStore()
</script>

<style scoped>
.counter {
  padding: 20px;
  text-align: center;
  border: 1px solid #ccc;
  border-radius: 8px;
  background-color: #fff;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.buttons {
  display: flex;
  gap: 20px;
  justify-content: center;
  align-items: center;
  margin-top: 15px;
}

button {
  padding: 10px 20px;
  font-size: 20px;
  cursor: pointer;
  border: none;
  background-color: #4CAF50;
  color: white;
  border-radius: 4px;
  transition: background-color 0.3s;
}

button:hover {
  background-color: #45a049;
}

.count {
  font-size: 24px;
  font-weight: bold;
  color: #333;
  min-width: 50px;
}

h2 {
  color: #333;
  margin-bottom: 15px;
}
</style>
