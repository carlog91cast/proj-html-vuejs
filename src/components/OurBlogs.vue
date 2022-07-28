 <template>
    <div class="container">
        <div class="title">
            <h6>READ FOR MORE JOYMENT</h6>
            <h1 class="m-5">
                Latest From
                <span>Our Blogs</span>
            </h1>
        </div>
        <!-- inserisco dinamicamente le card con un v for -->
        <div class="container mt-3">
            <div class="row justify-content-center">
                <div v-for="(artist, index) in artistList" :key="index" class="col-3 cart mx-3 rounded">
                    <div class="image">
                        <img class="rounded-top" :src="require(`../assets/img/${artist.img}`)" alt="">
                        <div v-show="hidden" class="free rounded-end">
                            FREE
                        </div>
                    </div>
                    <div class="text">
                        <div class="price">
                            {{ artist.price }}
                        </div>
                        <div class="description">
                            {{ artist.description }}
                        </div>
                        <div class="students mt-4">
                            <span>{{ artist.class }}</span>
                            <span>{{ artist.students }}</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'OurBlogs',
    data() {
        return {
            artistList: [
                {
                    img: 'course-02-480x298.jpg',
                    title: 'artist',
                    description: 'Brush strokes energize trees in paintings',
                    date: 'May 15, 2020',
                    views: '688 views',
                },
                {
                    img: 'stock-full-hd-03-480x298.jpg',
                    title: 'artist',
                    description: 'Pocket-Sized notebooks hold miniature paintings',
                    date: 'May 15, 2020',
                    views: '603 Views<',
                   
                },
                {
                    img: 'stock-full-hd-04-480x298.jpg',
                    title: 'artist',
                    description: 'connection Between Self-Portaits and identity',
                    date: 'May 15, 2020',
                    views: '397 Views',
                   
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import "~bootstrap/scss/bootstrap";
@import "../assets/style/common.scss";

.title {

    text-align: center;

    H6 {
        color: #6c6c6b;
        ;
    }

    h1 {
        font-weight: 600;
        font-size: 45px;

    }

    span {
        color: #1fad95;
    }
}

.cart {
    position: relative;
    background-color: white;
    padding: 0;

    .free {
        width: 50px;
        height: 25px;
        background-color: #ee7455;
        color: white;
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 10px;
        position: absolute;
        top: 0;
        right: 0;
    }
}

.cart:hover {
    background-color: #e2e2e0;
}

.price {
    font-size: 25px;
    font-weight: bold;
    color: #1fad95;
    margin-top: 15px;
    margin-left: 20px;
}

.price:hover {
    color: black;
}

.description {
    font-size: 15px;
    font-weight: 600;
    margin: 20px;
}

.students {
    color: #6c6c6b;

    span {
        margin-left: 20px;
    }
}
</style>
