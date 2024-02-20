<script >
import ComHeader from './components/ComponentHeader.vue'

import ComMain from  './components/ComponentMain.vue'

import ComFooter from './components/ComponentFooter.vue'

export default {
  components:{
    ComHeader,
    ComMain,
    ComFooter
  }
}
</script>

<template>
  <!-- componente header -->
  <ComHeader />
  <!-- componente main -->
  <ComMain />
  <!-- componente footer -->
  <ComFooter/>
</template>

<style lang="scss">
@use './style/general.scss' as *;
@use './style/partials/variable' as *;
// cartteristiche di h3 del progetto 
h3{
  color: $color_text;
}
</style>

<!-- non usare i nomi come i tag del html 
 -->