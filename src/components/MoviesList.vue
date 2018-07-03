<template>
  <div>
    {{movie.title}}
  </div>
</template>

<script>
import {apiKey} from '../assets/apiKey'

export default {
  name: "MoviesList",

  data () {
    return {
      movie: {},

    }
  },

  created: function () {
    this.fetchData()
  },


  methods: {
    fetchData: async function() {
      try {
        const res = await fetch(
          `https://api.themoviedb.org/3/movie/550?api_key=${apiKey}`
        );
        const movie  = await res.json()
        this.movie = movie
      } catch (e) {
        console.log("error", e);
      }
    }
  }


};
</script>

<style>
</style>
