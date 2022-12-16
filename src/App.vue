<script >
import AppHeader from './components/AppHeader.vue'

export default {
  name:'app',
   
  components : {
      AppHeader
  }
}

</script> 

<template>
  <div>
     <AppHeader />

  </div>
</template>
 
<style lang="scss"  >

  @use './styles/general.scss' as *;
  @use './styles/partials/variables.scss' as *;

    h1{
      color: $primary;
    }
</style>
