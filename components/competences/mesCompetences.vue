<template>
  <div :class="$style['partieCompetences']">
    <les-titres titre="Mes compétences" soustitre="Des prestations adaptées à vos envies !" />
    <div :class="$style['competences']">

    </div>
  </div>
</template>

<script>
import lesTitres from "../lesTitres.vue"
export default {
  components: {
    lesTitres
  }
}
</script>

<style module>
.partieCompetences{
  display: flex;
  flex-direction: column;
  align-items: center;
}

.competences{

}
</style>