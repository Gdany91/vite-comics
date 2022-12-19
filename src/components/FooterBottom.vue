<script>
    export default {
        name: 'FooterBottom',
        data() {
            return {
                social: [
                    {
                        img: "/public/footer-facebook.png"
                    },
                    {
                        img: "/public/footer-twitter.png"
                    },
                    {
                        img: "/public/footer-youtube.png"
                    },
                    {
                        img: "/public/footer-pinterest.png"
                    },
                    {
                        img: "/public/footer-periscope.png"
                    },
                ]
            }
        }
    }

</script>

<template>
    <div class="container">
        
        <a href="" class="signUp">SIGN-UP NOW!</a>
        
        <div class="social">

            <span class="text-follow">FOLLOW US</span>


            <a href="" v-for="(item, index) in social" :key="index">
                <img class="img" :src="item.img" alt="">
            </a>
        </div>

    </div>

</template>

<style lang="scss" scoped>

@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;


    .container{
        background-color: #303030;
        min-height: 100px; /* DEBUG */
        padding: $padding-container;
        @include flex-between-center;
    }

    .signUp{
        text-decoration: none;
        color: white;
        font-weight: bold;
        font-size: 18px;
        border: 2px solid $primary;
        padding: 15px;
        vertical-align: middle;
        height: 20px;
        display: flex;
        align-items: center;
        
            
    }

    .social{
        @include flex-between-center;

        gap: 1rem;

        span{
            font-weight: bold;
            color: $primary;
        }

    }


</style>