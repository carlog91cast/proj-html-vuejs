<template>
    <div class="jumbo-container">
        <div class="jumbo-text">
            <div class="text-a">
                <strong>Commerge Buisness</strong>
            </div>
            <div class="text-b">
                <strong>Distant Mentornig Program</strong>
            </div>

        </div>
        <div class="button">
            <a href="#">Download free guidebook </a>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ProjJumbo',
}

</script>

<style lang="scss" scoped>
@import "~bootstrap/scss/bootstrap";
@import "../assets/style/common.scss";

.jumbo-container {
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    background-image: url('../assets/img/home-3-hero-bg.jpg');
    color: white;
    text-align: center;
    padding: 150px 0;
}

.text-a {
    font-size: 35px;
    font-weight: 400;
}

.text-b {
    margin-top: 10px;
    font-size: 60px;
    font-weight: 100;
}

.button a {
    color: #1fad95;
    background-color: white;
    width: max-content;
    border-radius: 5px;
    padding: 23px 33px;
    font-weight: 700;
}

.button {
    margin-top: 40px;
}

.button a:hover {
    background-color: #1fad95;
    color: white;
    border: 1px solid #1fad95;
}
</style>
