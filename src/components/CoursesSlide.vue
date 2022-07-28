 <template>
    <div class="container">
        <div class="title">
            <h6>JOIN MAXCOACH AT BEST</h6>
            <h1 class="m-5">
                Latest Online
                <span>Courses</span>
            </h1>
        </div>
        <!-- inserisco dinamicamente le card con un v for -->
        <div class="container mt-3">
            <div class="row justify-content-center">
                <div v-for="(card, index) in cardList" :key="index" class="col-3 cart mx-3 rounded">
                    <div class="image">
                        <img class="rounded-top" :src="require(`../assets/img/${card.img}`)" alt="">
                        <div v-if="card.hidden" class="free rounded-end">
                            FREE
                        </div>
                    </div>
                    <div class="text">
                        <div class="price">
                            {{ card.price }}
                        </div>
                        <div class="description">
                            {{ card.description }}
                        </div>
                        <div class="students mt-4">
                            <span>{{ card.class }}</span>
                            <span>{{ card.students }}</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="container-select">
            <div class="select">
            </div>
            <div class="select-grey">

            </div>
            <div class="select-grey">

            </div>
            <div class="select-grey">

            </div>
            <div class="select-grey">

            </div>
        </div>
        <div class="end-text pb-5">
            Control your prefernce setting to get notified appropiate
            cousess <strong>View all coursess &RightArrow;</strong>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CoursesSlide',
    data() {
        return {
            cardList: [
                {
                    img: 'course-02-480x298.jpg',
                    price: '$40.00',
                    description: 'Learning to Write as a Professional Author',
                    class: '20 lessons',
                    students: '50 students',
                    hidden: false,
                },
                {
                    img: 'stock-full-hd-03-480x298.jpg',
                    price: '$0.00',
                    description: 'Customer- centric-info-Tech Strategies',
                    class: '24 lessons',
                    students: '769 students',
                    hidden: true,
                   
                },
                {
                    img: 'stock-full-hd-04-480x298.jpg',
                    price: '$19.00',
                    description: 'Open Programming Coursess for Everyone:Python',
                    class: '17 lessons',
                    students: '62 students',
                    hidden: false,
                   
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
.container-select{
	margin-top: 50px;
	display: flex;
	justify-content: center;
	align-items: center;
}
.select{
	width: 10px;
	height: 10px;
	border: 1px solid black;
	background-color: #000000;
	border-radius: 50%;
	margin-right: 15px;
}
.select-grey{
	width: 10px;
	height: 10px;
	border: 1px solid #d8d8d8;
	background-color: #d8d8d8;
	border-radius: 50%;
	margin-right: 15px;
}
.end-text{
	text-align: center;
	margin: 20px;
}
</style>
