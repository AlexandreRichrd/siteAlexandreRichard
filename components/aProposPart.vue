<template>
  <div id="about">
    <h1>À propos</h1>
    <h2>Alexandre RICHARD, 20 ans et toutes ses dents !</h2>
    <div class="logoEtTexte">
      <div class="texte">
        <h3>Un développeur web passionné !</h3>
        <p>Actuellement en BTS Systèmes Numériques, j’ai découvert  le développement web il y a 5 ans au CDI de mon lycée.</p>
        <p>Je me rappelle encore rentrer des cours et me précipiter sur l’ordinateur pour suivre des cours sur openclassroom.</p>
        <p>J’y ai appris les bases du HTML, du CSS, du PHP et du MySQL.</p>
        <p>J’ai au cours de ma deuxième année d’apprentissage,  j’ai commencé à investir dans des cours sur la plateforme Udemy avec des cours plus longs et plus précis. J’y ai d’ailleurs découvert Javascript.</p>
        <p>Puis au cours de la dernière année, j’ai commencé à suivre des cours sur Dyma où j’ai découvert le framework Javascript VueJS.</p>
      </div>
      <img src="@/static/images/logo.svg" alt="logo">
      <div class="texte">
        <h3>Mon expérience en développement</h3>
        <p>J’ai pendant plus de 4 ans développé des site web “pour le fun”.</p>
        <p>En effet, ma première mission de développeur web s’est déroulée durant mon stage de première année de BTS. J’ai en effet conçu une application web en HTML, CSS, PHP et MySQLi pour le collège et lycée Saint Gab’.</p>
        <p>Ce milieu m’ayant bien plu, j’ai décidé, en février 2022, de créer mon entreprise et c’est ce qui marqua le début de mon aventure d’auto-entrepreneur.</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
#about{
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 7rem 0 10rem 0;
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
}

h3{
  font-size: 1.5em;
  font-weight: 400;
  color: var(--sub-title-color);
}

p{
  color: var(--sub-title-color);
  width: 22rem;
  text-align: justify;
}

.logoEtTexte{
  margin-top: 10rem;
  display: flex;
  justify-content: center;
  gap: 10rem;
}
</style>