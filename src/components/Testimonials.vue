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
                    <h3 class="text-a"> <strong>Professional team of specialists and passionate mentors at
                            reach</strong> </h3>
                    <p class="text-b">Ineed to get a certification for English proficiency and MaxCoach is my best
                        choince.
                        Their tutors are smatrt and professional when dealing with students
                    </p>
                    <div class="d-flex">
                        <div class="image-down">
                            <img src="../assets/img/testimonial-avata-01.jpg" alt="image">

                        </div>
                        <div class="name">
                            <h3>Madley Pondor</h3>
                            <p>/IT specialists</p>
                        </div>
                    </div>
                </div>
                <div class="text-shadow-down">
                    <div class="image-down">
                        <img src="../assets/img/testimonial-avata-02.jpg" alt="inmg">
                    </div>
                    <div class="name-down">
                        <h3><strong>Mina Hollace</strong></h3>
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

// text-side
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

// shadow-card slide

// upper side
.text-shadow-up {
    padding: 15px;
    opacity: 0.4;
    background-color: #FFFFFF;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
}

// central side
.img-right {
    position: relative;

    .main-text {

        align-items: center;
        position: absolute;
        top: 72%;
        right: 64%;
        left: 47%;
        transform: translate(-50%, -50%);
        width: 100%;
        padding: 5%;
        background-color: #FFFFFF;
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);


        .text-a {
            font-size: 15px;
            color: #b5b5b5;
        }

        .text-b {
            margin-top: 20px;
            margin-bottom: 40px;
            color: #b5b5b5;
        }
    }
}


// lower size

.text-shadow-down {
    padding: 10px;
    position: absolute;
    bottom: -12%;
    width: 80%;
    display: flex;
    opacity: 0.4;
    background-color: #F8F8F8;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
    z-index: -1;

    h3 {
        font-size: 15px;
    }

    p {
        font-size: 10px;
        color: #747474;
    }
}

.image-down {
    width: 40px;
    height: 40px;
    margin-right: 15px;
    border-radius: 50%;
    overflow: hidden;

    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
}
</style>
