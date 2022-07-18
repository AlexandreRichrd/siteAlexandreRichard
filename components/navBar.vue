<template>
  <div id="bar">
    <computer-bar />
    <mobile-bar />
  </div>
</template>

<script>
import computerBar from './navbars/computerBar.vue'
import mobileBar from './navbars/mobileBar.vue'

export default {
  components:{
    computerBar,
    mobileBar
  }
}
</script>

<style>

</style>