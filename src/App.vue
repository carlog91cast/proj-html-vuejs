<template>
  <div id="app">
    <ProjHeader/>
    <ProjJumbo/>
    <ProjMain/>
    <ProjFooter/>
  </div>
</template>

<script>
import ProjHeader from './components/ProjHeader.vue'
import ProjJumbo from './components/ProjJumbo.vue'
import ProjMain from './components/ProjMain.vue'
import ProjFooter from './components/ProjFooter.vue'

export default {
  name: 'App',
  components: {
    ProjHeader,
    ProjJumbo,
    ProjMain,
    ProjFooter
  }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "./assets/style/common.scss";

</style>
