<script >

import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import FooterTop from './components/FooterTop.vue'
import FooterBottom from './components/FooterBottom.vue'


export default {
  name:'app',
   
  components : {
      AppHeader,
      AppMain,
      FooterTop,
      FooterBottom
  }
  
}

</script> 

<template>
  <header>
    <AppHeader />
  </header>

  <main>
    <AppMain />
  </main>
      
  <footer>
    <FooterTop />
    <FooterBottom />
  </footer>   
      
</template>
 
<style lang="scss"  >

  @use './styles/general.scss' as *;
  @use './styles/partials/variables.scss' as *;

 
   
</style>
