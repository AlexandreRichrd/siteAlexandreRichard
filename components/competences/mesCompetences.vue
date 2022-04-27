<template>
  <div :class="$style['partieCompetences']">
    <h1>Mes services</h1>
    <h2>Des prestations adaptées à vos envies !</h2>
    <div :class="$style['competences']">

    </div>
  </div>
</template>

<script>
  export default {
    
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