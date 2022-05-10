<template>
  <div id="mainColor">
    <h2>Theme principal :</h2>
    <div class="couleurs">
      <div class="troisCouleurs">
        <carre-couleur couleurhexa="4672E3" couleur="main"/>
        <carre-couleur couleurhexa="CAB785" couleur="marron"/>
        <carre-couleur couleurhexa="C15555" couleur="rouge"/>
      </div>
      <div class="troisCouleurs">
        <carre-couleur couleurhexa="9D53AF" couleur="violet"/>
        <carre-couleur couleurhexa="53AAAF" couleur="bleu"/>
        <carre-couleur couleurhexa="54AF53" couleur="vert"/>
      </div>
    </div>
  </div>
</template>

<script>
import carreCouleur from "./carreCouleur.vue"
export default {
  components: {
    carreCouleur
  }
}
</script>

<style>
#mainColor{
  display: flex;
  flex-direction: column;
}

h2{
  font-weight: 400;
}

.couleurs{
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.troisCouleurs{
  display: flex;
  justify-content: space-between;
  /* gap: 1.5rem; */
}
</style>