<template>
    <div class="container">
        <div class="d-flex justify-content-around align-items-center p-4">
            <div class="drop-list">
                <!-- menu list -->
                <ul class="d-flex mx-3">
                    <li v-for="(item, index) in dropList" :key="index">
                        <a class="text-dark" href="#">{{ item.text }}</a>
                    </li>
                </ul>
            </div>
            <!-- logo -->
            <div class="logo mb-2 mx-5">
                <img src="../assets/img/dark-logo.png" alt="logo">
            </div>
            <!-- icons -->
            <div class="search-section d-flex align-items-center">
                <div class="icons">
                    <i class="fa-solid fa-cart-shopping mx-3"></i>
                    <i class="fa-regular fa-circle-user mx-3"></i>
                </div>
                <div class="search d-flex align-items-center">
                    <input type="text" placeholder="search...">
                    <div class="lens">
                        <i class="fa-regular fa-magnifying-glass"></i>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ProjHeader',
    data() {
        return {
            dropList: [
                {
                    text: 'Home',
                    url: '#',
                    current: true
                },
                {
                    text: 'Pages',
                    url: '#',
                    current: true
                },
                {
                    text: 'Courses',
                    url: '#',
                    current: true
                },
                {
                    text: 'Features',
                    url: '#',
                    current: true
                },
                {
                    text: 'Blog',
                    url: '#',
                    current: true
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: true
                },

            ]
        }
    }
}


</script>

<style lang="scss" scoped>
@import "~bootstrap/scss/bootstrap";
@import "../assets/style/common.scss";

ul {
    li {
        margin-right: 30px;

    }
}

.logo {
    width: 13%;
}

.search {
    display: flex;
    background-color: #e2e2e0;
    border-radius: 10px;

    .lens {
        margin-right: 10px;
    }

    input {
        background-color: #e2e2e0;
        border: none;
        outline: none;
        resize: none;
        padding: 13px;
        color: black;
    }
}
</style>
