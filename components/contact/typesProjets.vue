<template>
  <div :class="$style['typeProjet']">
    <h4>Type de projet*</h4>
    <div :class="$style['cards']">
      <type-projet-card card-name="site vitrine"/>
      <type-projet-card card-name="landing page"/>
      <type-projet-card card-name="blog"/>
    </div>
  </div>
</template>

<script>
import typeProjetCard from "./typeProjetCard.vue"
  export default {
    components: {
      typeProjetCard
    }
  }
</script>

<style module>
.cards{
  display: flex;
  gap: 3rem;
}

.typeProjet{

}

.typeProjet h4{
  text-align: left;
  font-weight: 400;
}
</style>