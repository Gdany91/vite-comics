<script >
import CardContainer from './components/CardContainer.vue';
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'


export default {
  name:'app',
   
  components : {
      AppHeader,
      CardContainer,
      AppMain
  }
}

</script> 

<template>
  <div>
      <AppHeader />
      <CardContainer />
      <AppMain />
  </div>
</template>
 
<style lang="scss"  >

  @use './styles/general.scss' as *;
  @use './styles/partials/variables.scss' as *;

 
    h1{
      color: $primary;
    }
</style>
