<template>
  <main>
    <div class="wave">
        <WorkCulture/>
        <KnowHow/>
        <CoursesSlide/>
    </div>
  </main>
</template>

<script>
import WorkCulture from './WorkCulture.vue';
import KnowHow from './KnowHow.vue';
import CoursesSlide from './CoursesSlide.vue';


export default {
  name: 'ProjMain',
  components: {
    WorkCulture,
    KnowHow,
    CoursesSlide,
  }
 
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "../assets/style/common.scss";
</style>
