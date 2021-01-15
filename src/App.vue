<template>
  <div id="app">
    
    <HelloWorld msg="Welcome to Amalitech"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  background-color: rgb(252, 203, 207);
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #c51717;
  margin-top: 10px;
}
</style>
