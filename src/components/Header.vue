<template>
  <header>
    <h1><router-link to='/'>{{ title }}</router-link></h1>

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
      name: 'Craig',
      show: false
    };
  },
  computed: {}
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




