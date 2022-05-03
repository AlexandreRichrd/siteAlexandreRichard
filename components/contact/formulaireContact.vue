<template>
  <div :class="$style['formulaire']">
    <h1>Contactez moi via ce formulaire afin de <span>préciser votre solution web</span></h1>
    <types-projets />
  </div>
</template>

<script>
import typesProjets from "./typesProjets.vue"
  export default {
    components: {
      typesProjets
    }
  }
</script>

<style module>
.formulaire{
  background-color: var(--secondary-background-color);
  width: 30rem;
  height: 50rem;
  margin-bottom: 5rem;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.formulaire h1{
  font-weight: 400;
  font-size: 1.8em;
  width: 26rem;
  text-align: center;
}

.formulaire h1 span{
  color: var(--main-color);
}
</style>