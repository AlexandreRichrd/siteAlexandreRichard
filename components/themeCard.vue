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

  background-color: var(--background-color);
  width: 28.5rem;
  height: 11rem;
  border-radius: 20px;
  margin: 10rem;
}
</style>