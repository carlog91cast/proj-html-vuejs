<template>
  <main>
    <div class="wave">
        <WorkCulture/>
        <KnowHow/>
    </div>
  </main>
</template>

<script>
import WorkCulture from './WorkCulture.vue';
import KnowHow from './KnowHow.vue';


export default {
  name: 'ProjMain',
  components: {
    WorkCulture,
    KnowHow
  }
 
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "../assets/style/common.scss";
</style>
