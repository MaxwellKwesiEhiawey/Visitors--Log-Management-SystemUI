<template>
<div>
<div>
  <app-navibar />
    <div id="app"> 
    <Details msg="Welcome to Amalitech Front-desk"/>
  </div>
  <div class="conatiner home-conatiner">
    <app-file-loader />
  </div>
</div>
</div>

</template>

<script>
import Navibar from './components/Navibar.vue';
import Details from './components/Details.vue';
import FileLoader from './components/PageLoader';
export default {
  name: 'Home',
  components: {
    Details,
    'app-navibar': Navibar,
    'app-file-loader': FileLoader,
  }
}
</script>

<style>
#app {
  display: inline-block;
  background-color:#fdabab;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align:center;
  color: #c51717;
  border: 10px solid #690009;
  width: 100%;
  padding-right: 40px;
  position:inherit;
}
</style>
