<script>
    export default {
        name: 'AppMain',
        data() {
            return {
                items: [
                    {
                        img: "/public/buy-comics-digital-comics.png",
                        name: "DIGITAL COMICS"
                    },
                    {
                        img: "/public/buy-comics-merchandise.png",
                        name: "DC MERCHANDISE"
                    },
                    {
                        img: "/public/buy-comics-subscriptions.png",
                        name: "SUBSCRIPTION"
                    },
                    {
                        img: "/public/buy-comics-shop-locator.png",
                        name: "COMIC SHOP LOCATOR"
                    },
                    {
                        img: "/public/buy-dc-power-visa.svg",
                        name: "DC POWER VISA"
                    },
                ]
            }
    }
    }

</script>

<template>
    <div class="container">
        <ul>
            <li v-for="(item, index) in items" >
                <img :src="item.img" class="image">
                <a >
                    {{ item.name }}
                </a>
            </li>
        </ul>
        

    </div>

</template>

<style lang="scss" scoped>

    .container{
        background-color: #0282f9;
        min-height: 100px; /* DEBUG */
        padding: 0 15em;
        

    }

    ul{
        display: flex;
        justify-content: space-between;
        align-items: center;
        list-style-type: none;
        padding: 1rem 0;
       
        
    }

    li{
        display: flex;
        justify-content: space-between;
        align-items: center;
        color: white;

    }

 

    .image{
        width: 2.5rem;
        margin: 0.2rem 0.5rem;
    }


</style>