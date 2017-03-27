<template>
  <div id="app">
    <div id="details">
      <h1>Tic Tac Toe</h1>
    </div>
    <grid></grid>
  </div>
</template>

<script>
import Grid from './components/Grid.vue';

export default {
  name: 'app',
  components: { Grid },
  data() {
    return {
      matches: 0,
      wins: {
        O: 0,
        X: 0
      }
    }
  }
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

h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
