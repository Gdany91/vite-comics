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

    .container{
        background-color: #303030;
        min-height: 100px; /* DEBUG */
        padding: 0 15rem;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .signUp{
        text-decoration: none;
        color: white;
        font-weight: bold;
        font-size: 18px;
        border: 2px solid #0282f9;
        padding: 15px;
        vertical-align: middle;
        height: 20px;
        display: flex;
        align-items: center;
        
            
    }

    .social{
        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 1rem;

        span{
            font-weight: bold;
            color: #0282f9;
        }

    }


</style>