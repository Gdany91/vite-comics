<script>
    export default {
        name: 'FooterTop',
        data() {
            return {
                dcComics:
                    [
                        {
                            title: "DC COMICS",
                            list: [
                                {
                                    name: "Characters",
                                    
                                },
                                {
                                    name: "Comics",
                                    
                                },
                                {
                                    name: "Movies",
                                    
                                },
                                {
                                    name: "TV",
                                    
                                },
                                {
                                    name: "Games",
                                    
                                },
                                {
                                    name: "Videos",
                                    
                                },
                                {
                                    name: "News",
                                    
                                },
                            ],
                        },
                    ],
                dc: [
                    {
                        title: "DC",
                        list: [
                            {
                                name: "Terms Of Use",
                                
                            },
                            {
                                name: "Privacy policy (New)",
                                
                            },
                            {
                                name: "Ad Choices",
                                
                            },
                            {
                                name: "Advertising",
                                
                            },
                            {
                                name: "Jobs",
                                
                            },
                            {
                                name: "Subscriptions",
                                
                            },
                            {
                                name: "Talent WOrkshops",
                                
                            },
                            {
                                name: "CPSC Certificates",
                                
                            },
                            {
                                name: "Ratings",
                                
                            },
                            {
                                name: "Shop Help",
                                
                            },
                            {
                                name: "Contact Us",
                                
                            },
                        ]
                    }
                    ],

                sites: [
                            {
                            title: "SITES",
                                list: [
                                    {
                                        name: "DC",
                                        
                                    },
                                    {
                                        name: "MAD Magazine",
                                        
                                    },
                                    {
                                        name: "DC Kids",
                                        
                                    },
                                    {
                                        name: "DC Universe",
                                        
                                    },
                                    {
                                        name: "DC Power Visa",
                                        
                                    },
                                ]
                            }
                        ],
                shop:
                    [
                        {
                            title: "SHOP",
                            list: [
                                {
                                    name: "Shop DC",
                                    
                                },
                                {
                                    name: "Shop DC Collectibles",
                                    
                                },
                            ]
                        }
                    ],
            }
    }
    }

</script>

<template>
    
    <div class="container">
        <div class="container_menu">
            <div class="menu">
                <ul>
                    <li class="list" v-for="(item, index) in dcComics" >
                        <a href="" class="title ">{{ item.title }}</a>
                        <a href="" class= 'item' v-for="(items, index) in item.list">{{ items.name }} </a>

                    </li>
                </ul>
            </div>
            <div class="menu">
                <ul>
                    <li class="list" v-for="(item, index) in dc" >
                        <a href="" class="title ">{{ item.title }}</a>
                        <a href="" class= 'item' v-for="(items, index) in item.list">{{ items.name }} </a>

                    </li>
                </ul>
            </div>
            <div class="menu">
                <ul>
                    <li class="list" v-for="(item, index) in sites" >
                        <a href="" class="title ">{{ item.title }}</a>
                        <a href="" class= 'item' v-for="(items, index) in item.list">{{ items.name }} </a>

                    </li>
                </ul>
            </div>
            <div class="menu ">
                <ul>
                    <li class="list" v-for="(item, index) in shop" >
                        <a href="" class="title ">{{ item.title }}</a>
                        <a href="" class= 'item' v-for="(items, index) in item.list">{{ items.name }} </a>

                    </li>
                </ul>
            </div>

        </div>

        <img src="/public/dc-logo-bg.png" class="img">

    </div>
    


</template>

<style lang="scss" scoped>

@use '../styles/partials/variables.scss' as *;

    .container{
        background-image:  url("/public/footer-bg.jpg");
        height: 400px; 
        display: flex;
        justify-content: space-between;
        padding: $padding-container;
        overflow: hidden;
    }

   
     .container_menu {
        margin-top: 1rem;
        height: 100%;
        display: flex;
        flex-wrap: wrap;

    }

    .menu{
        width: calc(100% / 3);
        display: flex;
        flex-direction: column;

        a{
            text-decoration: none;

        }
    }

    img{
       
        height: 480px;
        margin-top: -50px;
    }

    .list{
        display: flex;
        flex-direction: column;
        
    }

    .item{
        color: gray;
    }

    .title {
        margin-bottom: 1rem;
        color: white;
    }
    
    


</style>