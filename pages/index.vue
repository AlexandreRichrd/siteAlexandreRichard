<template>
<div id="page">
  <header>
    <nav-bar />
  </header>
  <accueil-part />
  <div :class=" hover ? $style['theme2'] : $style['theme']" @mouseenter="reponsehover(true)" @mouseleave="reponsehover(false)">
    <theme-card-plus-bouton />
  </div>

  <a-propos-part />
  <!-- <mes-services /> -->
  <mes-competences />
  <mon-portfolio />
  <!-- <mon-contact /> -->
</div>
</template>


<script lang="ts">

import Vue from 'vue'
import navBar from '@/components/navBar.vue'
import accueilPart from '@/components/accueilPart.vue'
import aProposPart from '@/components/aProposPart.vue'
// import mesServices from '@/components/services/mesServices.vue'
import mesCompetences from '@/components/competences/mesCompetences.vue'
import monPortfolio from '@/components/portfolio/monPortfolio.vue'
// import monContact from '~/components/contact/monContact.vue'
import themeCardPlusBouton from '~/components/themeCard/themeCardPlusBouton.vue'


export default Vue.extend({
  name: 'IndexPage',
  components: {
    navBar,
    accueilPart,
    aProposPart,
    // mesServices,
    mesCompetences,
    monPortfolio,
    // monContact,
    themeCardPlusBouton
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

.theme{
  position: fixed;
  top:40%;
  transform: translateX(-28.5rem);
  transition: transform  0.2s ease-in-out;
}

.theme2{
  position: fixed;
  top:40%;
  transform: translateX(0rem);
  transition: transform  0.2s ease-in-out;
}
</style>