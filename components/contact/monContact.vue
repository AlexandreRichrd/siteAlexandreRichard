<template>
  <div :class="$style['partieContact']">
    <h1>Contact</h1>
    <div :class="$style['itemsContact']">
      <partie-gauche />
      <formulaire-contact />
    </div>
  </div>
</template>

<script>
import formulaireContact from "./formulaireContact.vue"
import partieGauche from "./partieGauche.vue"
  export default {
    components: {
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

h1{
  text-transform: uppercase;
  font-weight: 500;
  font-size: 2.5em;
}

h2{
  color: var(--sub-title-color);
  font-weight: 400;
  font-size: 2em;
  margin-bottom: 5rem;
}
</style>