<template>
  <header>
    <h1>{{ newTitle }}</h1>
  </header>
</template>

<script>
export default {
  name: "Header",
  props: {
    title: String
  },
  data() {
    return {
      name: 'Craig'
    }
  },
  computed: {
    newTitle: function() {
      console.log('this', this);
      return `${this.name} Orcutt `
    }
  }
};
</script>

<style scoped>
header {
  background-color: #111;
  padding: 1.5em;
  color: white;
}
h1 {
  margin: 0;
}
</style>
