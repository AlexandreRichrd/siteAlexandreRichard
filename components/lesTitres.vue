<template>
  <div class="titres">
    <h1>{{ titre }}</h1>
    <h2 v-if="soustitre!='none'">{{ soustitre }}</h2>
  </div>
</template>

<script>
  export default {
    props: {
      titre: {
        type: String,
        required: true
      },
      soustitre: {
        type: String,
        required: true
      }
    }
  }
</script>

<style scoped>
.titres{
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