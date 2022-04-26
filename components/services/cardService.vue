<template>
  <div id="card">
    <img :src="image" alt="">
    <div class="textes">
      <h2>{{ titre }}</h2>
      <p>{{ description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    titre: {
      type: String,
      required: true
    },
    description: {
      type: String,
      required: true
    },
    image: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
#card{
  background-color: #D6D6D6;
  height: 10rem;
  width: 30.5rem;
  border-radius: 19px;
  box-shadow: 1px 1px 4px rgba(0, 0, 0, 0.15);
  margin-bottom: 5rem;
  padding: 2.5rem;
  display: flex;
  gap: 3rem;
}

img{
  width: 6.35rem;
  height: 5.9rem;
}

h2{
  margin: 0;
  font-weight: 100;
  font-size: 2rem;
}

p{
  width: 18rem;
  text-align: justify;
  font-size: 1.1rem;
}
</style>