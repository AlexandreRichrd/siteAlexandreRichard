<template>
  <div :class="$style['partieContact']">
    <h1>Contact</h1>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style module>
.partieContact{
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
  margin-bottom: 5rem;
}
</style>