<template>
  <div id="card">
    <img src="@/static/images/dev-web.png" alt="">
    <div class="textes">
      <h2>Développement web</h2>
      <p>Mise en place d’une solution web répondant à votre besoin.
      Landing page, site vritrine, blog, ...</p>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
#card{
  background-color: #D6D6D6;
  height: 12rem;
  width: 30.5rem;
  border-radius: 19px;
  box-shadow: 1px 1px 4px rgba(0, 0, 0, 0.15);
  margin-bottom: 5rem;
  padding: 2.5rem;
  display: flex;
  gap: 3rem;
}

img{
  width: 5.85rem;
  height: 5.4rem;
}

h2{
  margin: 0;
}
</style>