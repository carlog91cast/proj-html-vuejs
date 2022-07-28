<template>
    <main>
        <div class="wave">
            <WorkCulture />
            <KnowHow />
            <CoursesSlide />
        </div>
        <div>
            <Testimonials />
            <TransformCard />
        </div>
        <div class="grey">
            <OurBlogs />
        </div>
        <div class="container mt-5">
            <div class="row">
                <div class="col-4 position-relative">
                    <img class="w-50 position-absolute square-sx" src="../assets/img/maxcoach-shape-07.png" alt="">
                </div>
                <div class="col-4">
                    <div class="mail">
                        <div class="text">
                            <div class="title">Subscribe <span>Newsletters</span></div>
                            <p>
                                Enter your email address to register to our nesletter subscription <br>
                                delivered on a regular basis!
                            </p>
                        </div>
                        <div class="container">
                            <div class="input-group mb-3 bar-email">
                                <input type="text" class="form-control" placeholder="Enter your email"
                                    aria-label="Recipient's username" aria-describedby="button-addon2">
                                <button class="btn button" type="button" id="button-addon2">Subscribe</button>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-4 position-relative">
                    <img class="w-50 square-point position-absolute" src="../assets/img/maxcoach-shape-05.png" alt="">
                    <img class="w-50 circle position-absolute" src="../assets/img/maxcoach-shape-02.png" alt="">
                </div>
            </div>
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
.grey {
     background-color: #FBFBFB 
}

.mail {
    padding-top: 100px;
    text-align: center;

    .text {
        .title {
            font-size: 35px;
            font-weight: bold;
            margin-bottom: 20px;

            span {
                color: #1fad95;
                font-weight: 300;
            }
        }

        p {
            font-size: 16px;
            color: #6c6c6b;
        }
    }

}


.bar-email {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-top: 45px;
    margin-bottom: 25px;

    input {
        width: 400px;
        height: 48px;
        background-color: #f5f5f5;
        border: none;
        resize: none;
        outline: none;
        font-size: 15px;
        padding-left: 20px;
    }

    .button {
        color: white;
        background-color: #1fad95;
        width: max-content;
        border-radius: 10px;
        font-size: 15px;
    }
}
.square-sx{
    top: 10%;
}

.square-point {
    top: 10%;
    right: 40%;
    left: 25%;
}

.circle {
    top: 36%;
    right: 32%;
    left: 33%;
}
</style>
