<template>
  <div id="app">
    <Step1/>
  </div>
</template>

<script>
import Step1 from './components/Step1.vue'

export default {
  name: 'App',
  components: {
    Step1
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
body {
  background-color:#FFF8DC;
}
</style>
