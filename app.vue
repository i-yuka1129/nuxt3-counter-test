<template>
  <div>
    <p>{{ counter }}</p>
    <button @click="counterStore.countUp">+</button>
    <button @click="counterStore.countDown">-</button>
    <button @click="counterStore.Reset">Rest</button>
  </div>
</template>
<script setup>
  const counterStore = useCounterState()
  const { counter } = counterStore
</script>
