<template>
  <div id="themeCard">
    <theme-card />
    <bouton-toogle-menu />
  </div>
</template>

<script>
import themeCard from '../themeCard.vue'
import boutonToogleMenu from './boutonToogleMenu.vue'

export default {
  components: {
    boutonToogleMenu,
    themeCard
  }
}
</script>

<style scoped>
@media only screen and (max-width: 600px){
  #themeCard{
    display: none;
  }
}
@media only screen and (min-width: 601px){
  #themeCard{
    display: flex;
  }
}


</style>