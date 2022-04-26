<template>
  <div id="partieServices">
    <h1>Mes services</h1>
    <h2>Des prestations adaptées à vos envies !</h2>
    <div class="cards">
      <div class="card2">
        <card-service 
          titre="Développement web" 
          description="Mise en place d’une solution web répondant à votre besoin. Landing page, site vritrine, blog, ..."
          image="https://hairturkey.fr/wp-content/uploads/2021/10/chauve.jpeg"
        />
        <card-service 
          titre="Design de votre site" 
          description="Création de maquette pour votre site et réalisation d’un design moderne."
          image="https://hairturkey.fr/wp-content/uploads/2021/10/chauve.jpeg"
        />
      </div>
      <div class="card2">
        <card-service 
          titre="Responsive design" 
          description="Création d’un site we compatible avec tous les support : ordinateur, téléphone et même télévision !"
          image="https://hairturkey.fr/wp-content/uploads/2021/10/chauve.jpeg"
        />
        <card-service 
          titre="Un site rapide" 
          description="Création d’un site web très rapide avec VueJs ou NuxtJs qui permettent de créer une single page application."
          image="https://hairturkey.fr/wp-content/uploads/2021/10/chauve.jpeg"
        />
      </div>
    </div>
  </div>
</template>

<script>
import cardService from './cardService.vue'

export default {
  components: {
    cardService
  }
}
</script>

<style scoped>
#partieServices{
  display: flex;
  flex-direction: column;
  align-items: center;
}

.card2{
  display: flex;
  justify-content: center;
  gap: 10rem
}

.cards{
  display: flex;
  flex-direction: column;
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