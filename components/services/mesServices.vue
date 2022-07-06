<template>
  <div id="partieServices">
    <les-titres titre="Mes services" soustitre="Des prestations adaptées à vos envies !" />
    <div class="cards">
      <div class="card2">
        <card-service
          titre="Développement web"
          description="Mise en place d’une solution web répondant à votre besoin. Landing page, site vritrine, blog, ..."
          image="https://zupimages.net/up/22/19/v0rq.png"
        />
        <card-service
          titre="Design de votre site"
          description="Création de maquette pour votre site et réalisation d’un design moderne."
          image="https://zupimages.net/up/22/19/t3mz.png"
        />
      </div>
      <div class="card2">
        <card-service
          titre="Responsive design"
          description="Création d’un site we compatible avec tous les support : ordinateur, téléphone et même télévision !"
          image="https://zupimages.net/up/22/19/4uy4.png"
        />
        <card-service
          titre="Un site rapide"
          description="Création d’un site web très rapide avec VueJs ou NuxtJs qui permettent de créer une single page application."
          image="https://zupimages.net/up/22/19/po7x.png"
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