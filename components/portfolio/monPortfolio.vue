<template>
  <div :class="$style['partiePortfolio']">
    <h1>Portfolio</h1>
    <h2>Des exemples pour cibler vos envies !</h2>
    <div :class="$style['items']">
      <div :class="$style['deuxItems']">
        <item-portfolio />
        <item-portfolio />
      </div>
      <div :class="$style['deuxItems']">
        <item-portfolio />
        <item-portfolio />
      </div>
    </div>
  </div>
</template>

<script>
import itemPortfolio from "./itemPortfolio.vue"
  export default {
    components:{
      itemPortfolio
    }
  }
</script>

<style module>
.partiePortfolio{
  display: flex;
  flex-direction: column;
  align-items: center;
}

.items{
  display: flex;
  flex-direction: column;
  gap: 3rem;
  margin: 3rem 0 ;
}

.deuxItems{
  display: flex;
  justify-content: center;
  gap: 6rem;
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