<template>
  <div id="app">
    
    <my-h1/>
  </div>
</template>

<script>
import myH1 from './components/my-h1.vue'

export default {
  components: {
    myH1
  }
}
</script>

<style >


*, *::before, *::after {
  box-sizing: border-box;
}

#app {
  max-width: 400px;
  margin: 0 auto;
  line-height: 1.4;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: $vue-blue;
}

h1 {
  text-align: center;
}
</style>