<template>
  <div :class="$style['partiePortfolio']">
    <les-titres titre="Portfolio" soustitre="Des exemples pour cibler vos envies !"/>
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
import lesTitres from "../lesTitres.vue"
import itemPortfolio from "./itemPortfolio.vue"
  export default {
    components:{
      itemPortfolio,
      lesTitres
    }
  }
</script>

<style module>

@media only screen and (max-width: 600px) {
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
    flex-direction: column;
    gap: 6rem;
  }
}
@media only screen and (min-width: 601px) {
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
}



</style>