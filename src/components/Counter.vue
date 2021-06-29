<script>
export default {
  props: {
    app: {
      type: Object,
      required: true
    }
  },
  data: () => ({
    count: 0
  }),
  methods: {
    incrementCount() {
      this.count++
    }
  },
  mounted() {
    console.log({ app })
  }
}
</script>

<template>
  <div class="counter">
    <h1>Counter</h1>
    <p>App: {{ app }} test</p>
    <p>Count: {{ count }}</p>
    <button @click="incrementCount">Increment</button>
  </div>
</template>

<style>
.counter {
  color: white;
  background-color: red;
  border: 2px solid #bada55;
}
</style>
