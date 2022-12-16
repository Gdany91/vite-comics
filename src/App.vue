<script >
import CardContainer from './components/CardContainer.vue';
import AppHeader from './components/AppHeader.vue'

export default {
  name:'app',
   
  components : {
      AppHeader,
      CardContainer
  }
}

</script> 

<template>
  <div>
     <AppHeader />
     <CardContainer />


  </div>
</template>
 
<style lang="scss"  >

  @use './styles/general.scss' as *;
  @use './styles/partials/variables.scss' as *;

    h1{
      color: $primary;
    }
</style>
