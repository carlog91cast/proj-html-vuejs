<template>
    <div class="container">
        <div class="row">
            <div class="col-6 img-left mt-4">
                <img src="../assets/img/stock-full-hd-11-670x450.jpg" style="width: 150%;" alt="img">
                <img class="range" src="../assets/img/icon-youtube-play.png" alt="img2">
                <img class="range-one" src="../assets/img/maxcoach-shape-05-100x100.png" alt="">
                <div class="img-around-left">
                    <img src="../assets/img/maxcoach-shape-07-150x150.png" alt="">
                </div>
            </div>
            <div class="col-6 text-section">
                <h6>HOW WE WORK</h6>
                <H1>Upgrade Your <br> Skills
                    <span>Upgrade <br> Your Life</span>
                </H1>
                <p>Opening up more opportunites in front of youy to get the <br> ticket to more enjoyable door in life.
                    Getting equipped
                    with <br> new skills for new set of insights into yoit career. <br> MaxCoach accompany learnes in
                    every stage
                    of learning
                </p>
                <div><a href=""><strong>Download free guidebook</strong></a></div>
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

.img-left {
    padding: 130px;
    position: relative;

    .range {
        width: 100px;
        border-radius: 10px;
        position: absolute;
        top: 43%;
        right: 28%;
        

    }

    .range-one {
        width: 24%;
        position: absolute;
        top: 30%;
        right: 70%;
        z-index: -1;
    }

    .img-around-left {
        width: 25%;
        position: absolute;
        bottom: 87px;
        right: -14%;
        z-index: -1;
    }
}
</style>
