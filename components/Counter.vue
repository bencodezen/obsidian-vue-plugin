<script>
export default {
  data: () => ({
    count: 0
  }),
  methods: {
    incrementCount() {
      this.count++
    }
  }
}
</script>

<template>
  <div class="counter">
    <h1>Counter</h1>
    <p>Count: {{ count }}</p>
    <button @click="incrementCount">Increment</button>
  </div>
</template>

<style>
.counter {
  color: white;
  background-color: black;
}
</style>
