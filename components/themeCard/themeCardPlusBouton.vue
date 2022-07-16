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
#themeCard{
  display: flex;
}

</style>