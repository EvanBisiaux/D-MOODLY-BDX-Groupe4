<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <MoodSlider msg='emotion'/>
</template>

<script>
import MoodSlider from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    MoodSlider  
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
