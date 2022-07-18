<template>
  <div :class="$style['btnPortfolio']">
    <a :class="$style['texteBouton']">Visiter</a>
  </div>
</template>

<script>
  export default {

  }
</script>

<style module>

@media only screen and (max-width: 990px) {
  .btnPortfolio{
    background-color: var(--main-color);
    width: 15rem;
    height: 44px;
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
  }

  .texteBouton{
    color: #FFF;
    font-size: 2em;
  }
}
@media only screen and (min-width: 991px) {
  .btnPortfolio{
    background-color: var(--main-color);
    width: 373px;
    height: 44px;
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
  }

  .texteBouton{
    color: #FFF;
    font-size: 2em;
  }
}

</style>