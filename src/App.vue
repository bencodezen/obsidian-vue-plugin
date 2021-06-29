<script>
export default {
  props: {
    app: {
      type: Object,
      required: true
    }
  },
  computed: {
    activeLeafData() {
      return this.app.workspace?.activeLeaf?.view?.data
    }
  }
}
</script>

<template>
  <h1>Root App</h1>
  <p>{{ activeLeafData }}</p>
</template>

<style></style>
