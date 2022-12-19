<script>
    export default {
        name: 'CardContainer',
    

        props: {
            cards: Array,
        },

        data() {
            return {
            }
        }
    }

</script>

<template>
    
    
        <ul>

            <li v-for="(card, index) in cards" :key="index">
                <a href="">
                    <img :src="card.thumb" alt="">
                    <div class="text">{{ card.series }}</div>
                </a>
            </li>

        </ul>
   

</template>

<style lang="scss" scoped>

@use '../styles/partials/variables.scss' as *;


   

        ul{
            flex-wrap: wrap;

            li{
                width: calc(100% / 6);
                position: relative;
                margin-bottom: 0.5rem;

                .text{
                    color: white;
                    text-decoration: none;
                    position: absolute;
                    bottom: 0.5rem;
                }
            }
        }
    

    

     
    


</style>