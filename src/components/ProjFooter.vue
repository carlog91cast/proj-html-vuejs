<template>
    <footer>
        <div class="container">
            <div class="row p-5">
                <div class="col-5">
                    <div class="address p-4">
                        <ul>
                            <h5>Address</h5>
                            <li>382 NE 191ist St# 97394 Miami, Fl 33179-3899</li>
                            <li>+1(305) 547-9909(9am - 5pm EST, Monday - Friday)</li>
                            <li>support@maxcoach.com</li>
                        </ul>
                    </div>
                    <div class="social">
                        <ul class="mb-5">
                            <li><img src="../assets/img/instagram-2-512.png" alt="img"></li>
                            <li><img src="../assets/img//facebook-3-512.png" alt="img"></li>
                            <li><img src="../assets/img/twitter-3-512.png" alt="img"></li>
                            <li><img src="../assets/img/1024px-Linkedin_icon.svg.png" alt="img"></li>

                        </ul>
                    </div>
                </div>
                <div class="col-7 list d-flex">
                    <ul>
                        <h5>Explore</h5>
                        <li v-for="obj, index in menuList" :key="index">
                            <a href="#">{{ obj.text }}</a>
                        </li>
                    </ul>
                    <ul class="second-list">
                        <li v-for="item, index in menuListOne" :key="index">
                            <a href="#">{{ item.text }}</a>
                        </li>
                    </ul>
                    <ul>
                        <h5>Information</h5>
                        <li v-for="info, index in menuListTwo" :key="index">
                            <a href="">{{ info.text }}</a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="text-footer-end">
                <p>@ 2020 Maxcoach. All rights Reserved</p>
            </div>
        </div>
    </footer>

</template>

<script>


export default {
    name: 'ProjFooter',
    data() {
        return {
            menuList: [
                {
                    text: 'Start here',
                    url: '#',
                    current: true
                },
                {
                    text: 'Blog',
                    url: '#',
                    current: true
                },
                {
                    text: 'About us',
                    url: '#',
                    current: true
                },

            ],
            menuListOne: [
                {
                    text: 'Success story',
                    url: '#',
                    current: true
                },
                {
                    text: 'Coursess',
                    url: '#',
                    current: true
                },
                {
                    text: 'Contact us',
                    url: '#',
                    current: true
                },
            ],
            menuListTwo: [
                {
                    text: 'Membership',
                    url: '#',
                    current: true
                },
                {
                    text: 'Punchase guide',
                    url: '#',
                    current: true
                },
                {
                    text: 'Privacy Policy',
                    url: '#',
                    current: true
                },
                {
                    text: 'Team of service',
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

footer {
    background-color: #171621;
}

.address {
    ul {
        h5 {
            color: white;
        }

        li {
            font-size: 13px;
            color: #b1b1b0;
            padding-top: 20px;
        }
    }

}

.social {
    margin-top: 15px;


    ul {
        display: flex;

    }

    li {
        width: 25px;
        margin-left: 20px;
    }
}

.list {
    padding-left: 100px;
    padding-top: 25px;

    ul {
        margin-right: 35px;

        h5 {
            color: white;
        }

        li {
            font-size: 13px;
            margin-right: 10px;
            margin-top: 10px;

            a {
                color: #b1b1b0;
            }
        }
    }
}

.second-list {
    margin-top: 33px;
}
.text-footer-end{
	color:  #b1b1b0;
	text-align: center;
	font-size: 12px;
	padding-bottom: 25px;
}
.linkedin{
    color: #8B8B90;
}
</style>
