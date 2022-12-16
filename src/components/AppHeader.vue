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
    padding: 0 15em;
    min-height: 80px; /* DEBUG */
    display: flex;
    justify-content: space-between;
    align-items: center;

 }

ul {
    display: flex;
   
    gap: 15px;
    list-style-type: none;
}

li{
     
     cursor: pointer;

     &:hover{
        border-bottom: 3px solid #0282f9;
     }
}

 .img-header{
    width: 3rem;
 }


</style>