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
</style>