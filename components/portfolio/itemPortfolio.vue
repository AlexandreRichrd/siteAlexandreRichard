<template>
  <div :class="$style['item']">
    <bouton-portfolio />
  </div>
</template>

<script>
import boutonPortfolio from "./boutonPortfolio.vue"
  export default {
    components: {
      boutonPortfolio
    }
  }
</script>

<style module>
.item{
  background-color: var(--secondary-background-color);
  width: 32.2rem;
  height: 14.5rem;
  display: flex;
  justify-content: center;
  align-items: flex-end;
  padding-bottom: 1rem;
}
</style>