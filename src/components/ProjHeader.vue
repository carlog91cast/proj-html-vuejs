<template>
    <div class="container">
        <div class="d-flex justify-content-around align-items-center p-4">
            <div class="drop-list">
                <!-- menu list -->
                <ul class="d-flex mx-3">
                    <li v-for="(item, index) in dropList" :key="index" class="dropdown">
                        <a class="text-dark dropdown-toggle" href="#">{{ item.text }}</a>
                    </li>
                </ul>
            </div>
            <!-- logo -->
            <div class="logo mb-2 mx-5">
                <img src="../assets/img/dark-logo.png" alt="logo">
            </div>
            <!-- icons -->
            <div class="search-section d-flex align-items-center">
                <div class="icons d-flex">
                    <img src="../assets/img/utent.svg" alt="">
                    <img src="../assets/img/Carrello.svg" alt="">
                </div>
                <div class="search d-flex align-items-center">
                    <input type="text" placeholder="search...">
                    <div class="lens">
                        <img src="../assets/img/search.svg" alt="">
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
    margin-right: 40px;

    li {
        margin-right: 40px;

        a {
            font-weight: 100;
            font-size: 14px;
        }

    }
}

.logo {
    img {
        width: 150%;
    }
}

.search-section {
    margin-left: 100px;


    .search {

        .lens {
            margin-right: 10px;
           
        }

        input {
            background-color: #F5F5F5;
            border: none;
            border-radius: 10px;
            outline: none;
            resize: none;
            padding: 10px;
            color: black;
        }
    }
}
</style>
