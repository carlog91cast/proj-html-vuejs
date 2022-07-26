<template>
  <div id="app">
    <ProjHeader/>
    <ProjMain/>
    <ProjFooter/>
  </div>
</template>

<script>
import ProjHeader from './components/ProjHeader.vue'
import ProjMain from './components/ProjMain.vue'
import ProjFooter from './components/ProjFooter.vue'

export default {
  name: 'App',
  components: {
    ProjHeader,
    ProjMain,
    ProjFooter
  }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "./assets/style/common.scss";

</style>
