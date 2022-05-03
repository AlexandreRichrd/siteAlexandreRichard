<template>
  <div id="partieServices">
    <les-titres titre="Mes services" soustitre="Des prestations adaptées à vos envies !" />
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
import lesTitres from '../lesTitres.vue'
import cardService from './cardService.vue'

export default {
  components: {
    cardService,
    lesTitres
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
</style>