<template>
  <header>
    <h1>{{title}}</h1>
  </header>
</template>

<script>
export default {
  name: 'Header',
  props: {
    title: String
  }
}
</script>

<style scoped>
  header {
    background-color: #111;
    padding: 1.5em;
    color: white
  }
  h1 {
    margin: 0
  }
</style>
