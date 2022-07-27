<template>
    <div class="container">
        <div class="row">
            <div class="col-6 text-section" style="padding-left:130px;">
                <h6>EVERYTHING IN <span>MACCOACH</span></h6>
                <H1>Learn about our <br>
                    <span>Work Culture</span> at <br>
                    MaxCoach
                </H1>
                <p>Spend some time to visit our website or head office and <br> discover our current couses,
                    enoliment procedure and <br> registration
                    deadline.we're opening new classes every <br>
                    beginning of each month
                </p>
                <div>Have questions? <a href=""><strong>Get Free Guide</strong></a></div>
            </div>
            <div class="col-6 img-right" style="padding-right: 130px;">
                <img src="../assets/img/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg" alt="img">
                <img class="range" src="../assets/img/about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg"
                    alt="img2">
                <img class="range-one" src="../assets/img/maxcoach-shape-07-100x100.png" alt="img3">
                <div class="img-around-right">
                    <img src="../assets/img/maxcoach-shape-02.png" alt="style">
                </div>
            </div>
        </div>
        <div class="data">
            <div class="number mx-4 px-4">
                <div class="color-a"><strong>129+</strong></div>
                <div class="color-b">ENROLED LEARNS</div>
            </div>
            <div class="number mx-4 px-4">
                <div class="color-a"><strong>80</strong></div>
                <div class="color-b">FINISHED SESSIONS</div>
            </div>
            <div class="number mx-4 px-4">
                <div class="color-a"><strong>4%</strong></div>
                <div class="color-b">SATISFACTION RATE</div>
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

.img-right {
    padding: 130px;
    position: relative;

    .range {
        width: 150px;
        border-radius: 10px;
        position: absolute;
        top: 50px;
        right: 50px;
    }
    .range-one{
        width: 16%;
        position: absolute;
        top: 13%;
        right: 22%;
        z-index: -1;
    }

    .img-around-right {
        position: absolute;
        bottom: 70px;
        right: 190px;
        z-index: -1;
    }
}

.data {
    display: flex;
    justify-content: center;

    .number {
        margin-left: 50px;

        .color-a {
            color: #1fad95;
            font-size: 45px;
            text-align: center;
        }

        .color-b {
            font-size: 20px;
            margin-top: 10px;
            color: #6c6c6b;
        }
    }

}
</style>
