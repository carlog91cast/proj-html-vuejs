<template>
    <main>
        <div class="wave">
            <WorkCulture />
            <KnowHow />
            <CoursesSlide />
        </div>
        <div>
            <Testimonials />
        </div>
    </main>
</template>

<script>
import WorkCulture from './WorkCulture.vue';
import KnowHow from './KnowHow.vue';
import CoursesSlide from './CoursesSlide.vue';
import Testimonials from './Testimonials.vue';


export default {
    name: 'ProjMain',
    components: {
        WorkCulture,
        KnowHow,
        CoursesSlide,
        Testimonials,
    }

}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "../assets/style/common.scss";

.wave {
    background-color: #FBFBFB
}
</style>
