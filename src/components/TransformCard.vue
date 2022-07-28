<template>
    <div class="container">
        <div class="row">
            <div class="col-6 img-left mt-4">
                <img src="../assets/img/home-3-team-image.png" style="width: 150%;" alt="img">
                <img class="range" src="../assets/img/maxcoach-shape-05-150x150.png" alt="img2">
                <img class="range-one" src="../assets/img/maxcoach-shape-07-150x150.png" alt="">
                <div class="img-around-right">
                    <img src="../assets/img/maxcoach-shape-01.png" alt="">
                </div>
            </div>
            <div class="col-6 text-section">
                <h6>EVERYTHING IN <span>MACCOACH</span></h6>
                <H1>We're Here To <br>
                    <span>transform</span> You! <br>

                </H1>
                <p>As learners, people can enjoy great companionship from <br>
                    MaxCoach mentors and educators. we can help you <br>
                    develop and grow at your best
                </p>
                <div class="button">
                    <a href="#">Get Free Guide</a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'KnowHow',
}
</script>

<style lang="scss" scoped>
@import "~bootstrap/scss/bootstrap";
@import "../assets/style/common.scss";

.text-section {
    padding: 130px;
    position: relative;
    margin-top: 10%;

    .range {
        width: 50px;
        position: absolute;
        top: 50%;
        right: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
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
            font-weight: 400;
        }
    }

    p {
        color: #6c6c6b;
    }

    .button a {
        background-color: #1fad95;
        color: white;
        width: max-content;
        border-radius: 5px;
        padding: 20px 30px;
        font-weight: 700;
    }

    .button {
        margin-top: 40px;
    }

    .button a:hover {
        background-color:#b1b1b0;
        color: #1fad95;
        border: 1px solid #1fad95;
    }
}

.img-left {
    padding: 130px;
    position: relative;

    .range {
        width: 200px;
        position: absolute;
        top: 34%;
        right: 72%;


    }

    .range-one {
        width: 27%;
        position: absolute;
        top: 70%;
        right: 14%;
        z-index: -1;
    }

    .img-around-right {
        width: 25%;
        position: absolute;
        bottom: 87px;
        left: -9%;
        z-index: -1;
    }
}
</style>
