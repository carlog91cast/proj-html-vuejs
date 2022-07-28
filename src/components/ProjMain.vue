<template>
    <main>
        <div class="wave">
            <WorkCulture />
            <KnowHow />
            <CoursesSlide />
        </div>
        <div>
            <Testimonials />
            <TransformCard/>
        </div>
        <div class="grey">
            <OurBlogs/>
        </div>
    </main>
</template>

<script>
import WorkCulture from './WorkCulture.vue';
import KnowHow from './KnowHow.vue';
import CoursesSlide from './CoursesSlide.vue';
import Testimonials from './Testimonials.vue';
import TransformCard from './TransformCard.vue';
import OurBlogs from './OurBlogs.vue';


export default {
    name: 'ProjMain',
    components: {
    WorkCulture,
    KnowHow,
    CoursesSlide,
    Testimonials,
    TransformCard,
    OurBlogs,
}

}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "../assets/style/common.scss";

.wave .grey {
    background-color: #FBFBFB
}

</style>
