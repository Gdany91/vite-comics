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

@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;


.container{
    padding: $padding-container;
    min-height: 80px; /* DEBUG */
    @include flex-between-center;


 }

ul {
    display: flex;
    
    gap: 15px;
    list-style-type: none;
    align-items: center;
}

li{
     
     cursor: pointer;

     &:hover{
        color: $primary;
        border-bottom: 3px solid $primary;
     }
}

 .img-header{
    width: 3rem;
 }


</style>