<template>
  <div :class="$style['partieContact']">
    <les-titres titre="Contact" soustitre="none" />
    <div :class="$style['itemsContact']">
      <partie-gauche />
      <formulaire-contact />
    </div>
  </div>
</template>

<script>
import lesTitres from "../lesTitres.vue"
import formulaireContact from "./formulaireContact.vue"
import partieGauche from "./partieGauche.vue"
  export default {
    components: {
      lesTitres,
      formulaireContact,
      partieGauche
    }
  }
</script>

<style module>
.partieContact{
  display: flex;
  flex-direction: column;
  align-items: center;
}

.itemsContact{
  display: flex;
  justify-content: center;
  gap: 4rem;
}
</style>