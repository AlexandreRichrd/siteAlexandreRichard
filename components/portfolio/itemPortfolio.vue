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
@media only screen and (max-width: 990px) {
  .item{
    background-color: var(--portfolio-background-color);
    width: 20rem;
    height: 10rem;
    display: flex;
    justify-content: center;
    align-items: flex-end;
    padding-bottom: 1rem;
    background-image: url('@/static/images/portfolio/portfolio.png');
    background-size:75% ;
    background-position-y: top;
    background-position-x: center;
    background-repeat: no-repeat;
  }
}
@media only screen and (min-width: 991px) {
  .item{
    background-color: var(--portfolio-background-color);
    width: 32.2rem;
    height: 14.5rem;
    display: flex;
    justify-content: center;
    align-items: flex-end;
    padding-bottom: 1rem;
    background-image: url('@/static/images/portfolio/portfolio.png');
    background-size:75% ;
    background-position-y: top;
    background-position-x: center;
    background-repeat: no-repeat;
  }
}


</style>