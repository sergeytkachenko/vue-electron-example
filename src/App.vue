<template>
  <div id="app">
    <input v-model="src">
    <site :src="src"></site>
  </div>
</template>

<script>
import Site from './components/Site.vue'

export default {
  name: 'app',
  components: {
    Site
  },
  data: () => ({
    src: "https://www.whatsmybrowser.org/"
  })
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
