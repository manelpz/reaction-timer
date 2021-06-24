<template>
<h1>Ninja reaction Timer </h1>
<button @click="start">play</button>
</template>

<script>

export default {
  name: 'App',
  components: {
  },
  data(){
    return {
      isPlaying: false,
      delay:null
    }
  },
  methods:{
    start(){
      this.delay = 2000 + Math.random() * 5000
      this.isPlaying = true
      console.log(this.delay)
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-fonAt-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #444;
  margin-top: 60px;
}
</style>
