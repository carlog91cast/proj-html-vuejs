 <template>
    <div class="container">
        <div class="title mt-3">
            <h6>READ FOR MORE JOYMENT</h6>
            <h1 class="m-5">
                Latest From
                <span>Our Blogs</span>
            </h1>
        </div>
        <!-- inserisco dinamicamente le card con un v for -->
        <div class="container mt-3">
            <div class="row justify-content-center">
                <div v-for="(artist, index) in artistList" :key="index" class="col-3 cart mx-2 rounded">
                    <div class="image">
                        <img class="rounded-top" :src="require(`../assets/img/${artist.img}`)" alt="">
                    </div>
                    <div class="text p-1">
                        <div class="price">
                            {{ artist.title }}
                        </div>
                        <div class="description">
                            {{ artist.description }}
                        </div>
                        <div class="students mt-5">
                            <span>{{ artist.date }}</span>
                            <span class="mx-5">{{ artist.views }}</span>
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
                    img: 'artist-blog-03-480x325.jpeg',
                    title: 'ARTIST',
                    description: 'Brush strokes energize trees in colorful paintings',
                    date: 'May 15, 2020',
                    views: '688 views',
                },
                {
                    img: 'artist-blog-01-480x325.jpg',
                    title: 'ARTIST',
                    description: 'Pocket-Sized notebooks hold miniature paintings',
                    date: 'May 15, 2020',
                    views: '603 Views',
                   
                },
                {
                    img: 'artist-blog-02-480x325.jpg',
                    title: 'ARTIST',
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
    width: 30%;
    .text{
        margin-left: 8px;
    }
   
}

.cart:hover {
    background-color: #e2e2e0;
}

.price {
    font-size: 15px;
    font-weight: 300;
    color:#6c6c6b;
    margin-top: 15px;
}

.price:hover {
    color: black;
}

.description {
    font-size: 15px;
    font-weight: 600;
    margin-top: 15px;
}

.students {
    color: #6c6c6b;

}
</style>
