<template>
  <div id="app">
    <!--<img src="./assets/logo.png">-->
    <Nav/>
    <NormalLine/>
    <router-view/>
  </div>
</template>

<script>
import Nav from "./components/Nav"
import NormalLine from "./components/NormalLine"
export default {
  name: 'App',
  components: {NormalLine, Nav}
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
