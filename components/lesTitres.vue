<template>
  <div class="titres">
    <h1>{{ titre }}</h1>
    <h2 v-if="soustitre!='none'">{{ soustitre }}</h2>
    <hr>
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
@media only screen and (max-width: 600px) {
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
  margin-bottom: 3rem;
  text-align: center;
  width: 70%;
}

hr{
  background-color: var(--main-color);
  border: none;
  width: 5rem;
  height: 0.3rem;
  margin-bottom: 5rem;
}
}
@media only screen and (min-width: 601px) {
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
  margin-bottom: 3rem;
}

hr{
  background-color: var(--main-color);
  border: none;
  width: 5rem;
  height: 0.3rem;
  margin-bottom: 5rem;
}
}

</style>