<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-2">
                    
                </div>
                <div class="col-10"></div>
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
            menuListaTwo: [
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
</style>
