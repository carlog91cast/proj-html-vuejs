<template>
    <div class="container">
        <div class="row">
            <div class="col-6 text-section" style="padding-left:130px;">
                <h6>TESTIMONIALS</h6>
                <H1>Why Do Peaple <br>
                    <span>*Hearts*</span> Us?<br>
                </H1>
                <p>Seeking for verbals of our service quality? Find them here. <br> Everything is transparent and
                    straightforward for your sense <br> of justification
                </p>
                <div><a href=""><strong>Get Free Guide &RightArrow;</strong></a></div>
            </div>
            <div class="col-6 img-right" style="padding-right: 130px;">
                <div class="text-shadow-up">
                    <div><strong>The MaxCoach team realliy hard to ensure hight level of quality</strong>
                        <br> am happy with their arrangement of lessons and subject they
                    </div>
                </div>
                <div class="main-text">
                    <h3 class="ha">Professional team of specialists and passionate mentors at reach</h3>
                    <p class="hp">Ineed to get a certification for English proficiency and MaxCoach is my best choince.
                        Their tutors are smatrt and professional when dealing with students
                    </p>
                    <div class="profile">
                        <div class="image">
                            <img src="../assets/img/testimonial-avata-01.jpg" alt="image">

                        </div>
                        <div class="name">
                            <h3>Madley POndor</h3>
                            <p>/IT specialists</p>
                        </div>
                    </div>
                </div>
                <div class="text-shadow-down">
                    <div class="image-down">
                        <img src="../assets/img/testimonial-avata-02.jpg" alt="inmg">
                    </div>
                    <div class="name-down">
                        <h3>Mina Hollace</h3>
                        <p>/Freelancer</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>



export default {
    name: 'WorkCulture',


}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "../assets/style/common.scss";

.text-section {
    padding: 130px;
    position: relative;

    .img-around {
        position: absolute;
        bottom: 10%;
        right: 10%;
    }


    h6 {
        font-size: 16px;
        color: #b1b1b0;
        margin-bottom: 20px;

        span {
            color: #6c6c6b;
        }
    }

    h1 {
        font-size: 45px;
        font-weight: 600;
        margin-bottom: 20px;

        span {
            color: #1fad95;
            ;
        }
    }

    p {
        color: #6c6c6b;
    }

    div {
        color: #6c6c6b;

        a {
            color: #1fad95;
        }
    }
}
</style>
