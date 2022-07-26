<template>
  <div id="app">
    <ProjHeader/>
    <ProjMain/>
    <ProjFooter/>
  </div>
</template>

<script>
import ProjHeader from './components/ProjHeader.vue'
import ProjMain from './components/ProjHeader.vue'
import ProjFooter from './components/ProjHeader.vue'

export default {
  name: 'App',
  components: {
    ProjHeader,
    ProjMain,
    ProjFooter
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
