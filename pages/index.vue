<template>
<div id="page">
  <header>
    <nav-bar />
  </header>
  <accueil-part />
  <a-propos-part />
</div>
</template>

<script lang="ts">
import Vue from 'vue'
import navBar from '@/components/navBar.vue'
import accueilPart from '@/components/accueilPart.vue'
import aProposPart from '@/components/aProposPart.vue'

export default Vue.extend({
  name: 'IndexPage',
  components: {
    navBar,
    accueilPart,
    aProposPart
  },
  layout () {
    return 'defaultPage'
  }
})
</script>

<style scoped>
#page{
  margin: 0;
  background-color: var(--background-color);
}

</style>