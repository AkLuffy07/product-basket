<template>
  <div id="app">
    <navHeader />
  </div>
</template>

<script>
import navHeader from './components/navHeader.vue';

export default {
  name: 'App',
  components: {
    navHeader,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
