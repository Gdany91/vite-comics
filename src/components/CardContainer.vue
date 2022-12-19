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
    
    <div class="container">
        <ul>

            <li v-for="(card, index) in cards" :key="index">
                <a href="">
                    <img :src="card.thumb" alt="">
                    <div class="text">{{ card.series }}</div>
                </a>
            </li>

        </ul>
        

    </div>

</template>

<style lang="scss" scoped>

@use '../styles/partials/variables.scss' as *;


    .container{
        background-color: black;
        min-height: 80px; /* DEBUG */
        padding: $padding-container;
    }


</style>