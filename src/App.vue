<template>
  <LoadingScreen :status="loaded"/>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import LoadingScreen from './components/LoadingScreen.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    LoadingScreen
  },
  data () {
    return {
      loaded: 1
    }
  },
  mounted () {
    setTimeout(() => {
      this.loaded = 0
    }, 2000);
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
