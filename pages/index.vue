<template>
<div id="page">
  <header>
    <nav-bar />
  </header>
  <accueil-part />
  <bouton-toogle-menu @souris-dessus="reponsehover"/>
  <div :class="hover ? $style['modalevisible'] : $style['modaleinvisible']">
    <theme-card />
  </div>
  <a-propos-part />
  <mes-services />
  <mes-competences />
  <mon-portfolio />
  <mon-contact />
</div>
</template>

<script lang="ts">

import Vue from 'vue'
import navBar from '@/components/navBar.vue'
import accueilPart from '@/components/accueilPart.vue'
import aProposPart from '@/components/aProposPart.vue'
import mesServices from '@/components/services/mesServices.vue'
import mesCompetences from '@/components/competences/mesCompetences.vue'
import monPortfolio from '@/components/portfolio/monPortfolio.vue'
import monContact from '~/components/contact/monContact.vue'
import themeCard from '~/components/themeCard.vue'
import boutonToogleMenu from '~/components/themeCard/boutonToogleMenu.vue'



export default Vue.extend({
  name: 'IndexPage',
  components: {
    navBar,
    accueilPart,
    aProposPart,
    mesServices,
    mesCompetences,
    monPortfolio,
    monContact,
    themeCard,
    boutonToogleMenu
  },
  layout () {
    return 'defaultPage'
  },
  data(){
    return{
      hover: false,

    }
  },
  methods:{
    reponsehover(reponse: boolean){
      this.hover = reponse
      console.log(reponse)
    }
  }
})
</script>

<style module>
#page{
  margin: 0;
  background-color: var(--background-color);
}

.modalevisible{
  display: block
}

.modaleinvisible{
  display: none
}

</style>