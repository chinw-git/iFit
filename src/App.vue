<template>
  <div id="app">
    <Header v-if="$route.meta.header === 1">></Header>
    <router-view></router-view>
  </div>
</template>


<script>
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    Header
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Fjalla+One&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Rubik&display=swap');

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>