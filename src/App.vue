<script >
import CardContainer from './components/CardContainer.vue'
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import FooterTop from './components/FooterTop.vue'
import FooterBottom from './components/FooterBottom.vue'


export default {
  name:'app',
   
  components : {
      AppHeader,
      CardContainer,
      AppMain,
      FooterTop,
      FooterBottom
  }
}

</script> 

<template>
  <div>
      <AppHeader />
      <CardContainer />
      <AppMain />
      <FooterTop />
      <FooterBottom/>

  </div>
</template>
 
<style lang="scss"  >

  @use './styles/general.scss' as *;
  @use './styles/partials/variables.scss' as *;

 
    h1{
      color: $primary;
    }
</style>
