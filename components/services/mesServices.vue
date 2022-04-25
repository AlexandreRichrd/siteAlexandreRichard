<template>
  <div id="partieServices">
    <h1>Mes services</h1>
    <h2>Des prestations adaptées à vos envies !</h2>
    <div class="card12">
      <card-service />
    </div>
  </div>
</template>

<script>
import cardService from './cardService.vue'

export default {
  components: {
    cardService
  }
}
</script>

<style scoped>
#partieServices{
  display: flex;
  flex-direction: column;
  align-items: center;
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
}
</style>