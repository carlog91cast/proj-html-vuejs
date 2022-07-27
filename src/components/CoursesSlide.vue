 <template>
    <div class="container">
        <div class="title">
            <h1>
                Latest Online
                <span>Courses</span>
            </h1>
        </div>
        <!-- inserisco dinamicamente le card con un v for -->
        <div class="container">
            <div class="row">
                <div class="col-4">
                    <div class="image">
                        <img src="" alt="img">
                        <div class="free">
                            FREE
                        </div>
                    </div>
                    <div class="text">
                        <div class="price">

                        </div>
                        <div class="description">

                        </div>
                        <div class="class">
                            <span></span>
                            <span></span>
                        </div>
                    </div>
                </div>
            </div>
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
                },
                {
                    img: 'stock-full-hd-03-480x298.jpg',
                    price: '$0.00',
                    description: 'Customer- centric-info-Tech Strategies',
                    class: '24 lessons',
                    students: '769 students',
                },
                {
                    img: 'stock-full-hd-04-480x298.jpg',
                    price: '$19.00',
                    description: 'Open Programming Coursess for Everyone:Python',
                    class: '17 lessons',
                    students: '62 students',
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "~bootstrap/scss/bootstrap";
@import "../assets/style/common.scss";

.title {

    text-align: center;

    h1 {
        font-weight: 600;
        font-size: 45px;
    }

    span {
        color: #1fad95;
    }
}
</style>
