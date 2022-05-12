<template>
  <div :class="$style['card']">
    <light-dark-mode />
    <main-color />
  </div>
</template>

<script>
import lightDarkMode from './themeCard/lightDarkMode.vue'
import mainColor from './themeCard/mainColor.vue'

export default {
  components: {
    lightDarkMode,
    mainColor
  }
}
</script>

<style module>
.card{
  display: flex;
  justify-content: center;
  gap: 2rem;

  background-color: rgb(202, 202, 202);
  width: 28.5rem;
  height: 11rem;
  border-radius: 20px;
  
  position: fixed;
  top: 50%;
  left: 0;
}
</style>