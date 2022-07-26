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

</style>
