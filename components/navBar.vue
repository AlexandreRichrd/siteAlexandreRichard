<template>
  <header>
    <img src="../static/images/logo.svg" alt="logo" class="logo">
    <ul>
      <li>Accueil</li>
      <li>À propos</li>
      <li>Services</li>
      <li>Compétences</li>
      <li>Portfolio</li>
      <li>Contact</li>
    </ul>
    <div class="social">
      <a href="https://www.instagram.com/alexandre_richrd/"><img src="@/static/images/instagram.png" alt="Lien Instagram" /></a>
      <a href="https://www.linkedin.com/in/alexandre-richard-5035a3194"><img src="@/static/images/linkedin.png" alt="Lien LinkedIn" /></a>
    </div>
  </header>
</template>

<script>
export default {

}
</script>

<style scoped>
header{
  background-color: rgba(172, 172, 172, 0.1);
  height: 6.5rem;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 23rem;
  position: fixed;
  width: 100%;
}

.logo{
  width: 5.5rem;
}

ul{
  display: flex;
  gap: 5rem
}

li{
  list-style-type: none;
  font-size: 1.2rem;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  color: #DFDFDF;
}

.social{
  display: flex;
  gap: 2rem
}

.social img{
  width: 1.5rem;
  opacity: 80%
}


</style>