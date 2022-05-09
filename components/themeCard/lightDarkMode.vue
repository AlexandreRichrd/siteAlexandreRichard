<template>
  <div id="mode">
    <h2>Mode jour / nuit</h2>
    <le-switch />
  </div>
</template>

<script>
import leSwitch from './leSwitch.vue'
export default {
  components: {
    leSwitch
  }
}
</script>

<style>

#mode {
  display: flex;
  flex-direction: column;
  align-items: center;
}

 #mode h2{
  font-weight: 400;
}
</style>