<script>
    export default {
        name: 'AppHeader',
        data() {
            return {
                
                link: [
                    {
                    name: "CHARACTERS",
                    
                    },
                    {
                    name: "COMICS",
                    
                    },
                    {
                    name: "MOVIES",
                    
                    },
                    {
                    name: "TV",
                    
                    },
                    {
                    name: "GAMES",
                    
                    },
                    {
                    name: "COLLECTIBLES",
                    
                    },
                    {
                    name: "VIDEOS",
                    
                    },
                    {
                    name: "FANS",
                    
                    },
                    {
                    name: "NEWS",
                    
                    },
                    {
                    name: "SHOP",
                    
                    },
                ]
            }
        },

    }
</script>

<template>
    <header>
        <div class="container">
            <div>
                <img src="../../public/dc-logo.png" class="img-header">
            </div>

            <ul class="list">
                <li v-for="(item, index) in link"  >
                    {{item.name}}
                </li>
            </ul>

        </div>

    </header>
</template>

<style lang="scss" scoped>

 .container{
    background-color: rebeccapurple; /* DEBUG */
    min-height: 80px; /* DEBUG */
    display: flex;
    justify-content: space-evenly;
    align-items: center;

 }

 ul {
    display: flex;
    
    gap: 15px;
    list-style-type: none;
 }


</style>