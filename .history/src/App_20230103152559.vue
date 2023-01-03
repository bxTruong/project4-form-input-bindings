<template>
  <Quizform/>
</template>

<script>
import Quizform from './components/Quizform.vue'

export default {
  name: 'App',
  components: {
    Quizform
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
