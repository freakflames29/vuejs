<template>

  <Hi name="Sourav" title="Das" age='20'/>

  <!-- <Bn/> -->
  <Sd lang="Rails and vue"/>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Hi from './components/Hi'
import Bn from './components/Bn'
import Sd from './components/Sd'
import './assets/st.css'

export default {
  name: 'App',
  components: {
    Hi,
    Bn,
    Sd
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
