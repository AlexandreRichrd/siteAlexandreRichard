<template>
  <header :class="scroll ? $style['navbarCouleur'] : $style['navbarTransparent']">
    <img src="/images/logo.svg" alt="logo" :class="$style['logo']">
    <ul :class="$style['listeNavbar']">
      <li :class="scroll ? $style['membreListeNavbarCouleur'] : $style['membreListeNavbar']">Accueil</li>
      <li :class="scroll ? $style['membreListeNavbarCouleur'] : $style['membreListeNavbar']">À propos</li>
      <!-- <li :class="scroll ? $style['membreListeNavbarCouleur'] : $style['membreListeNavbar']">Services</li> -->
      <li :class="scroll ? $style['membreListeNavbarCouleur'] : $style['membreListeNavbar']">Compétences</li>
      <li :class="scroll ? $style['membreListeNavbarCouleur'] : $style['membreListeNavbar']">Portfolio</li>
      <!-- <li :class="scroll ? $style['membreListeNavbarCouleur'] : $style['membreListeNavbar']">Contact</li> -->
    </ul>
    <div :class="$style['social']">
      <a href="https://www.instagram.com/alexandre_richrd/"><img src="/images/instagram.png" alt="Lien Instagram" :class="$style['imageSocial']" /></a>
      <a href="https://www.linkedin.com/in/alexandre-richard-5035a3194"><img src="/images/linkedin.png" alt="Lien LinkedIn" :class="$style['imageSocial']" /></a>
    </div>
  </header>
</template>

<script>
export default {
  data(){
    return{
      scroll: false,
      theme: ''
    }
  },
  mounted(){
    document.addEventListener("scroll", () => {

      if(window.scrollY === 0){
        this.scroll = false
      }else{
        this.scroll = true
      }
    })
  }
}
</script>

<style module>

@media only screen and (max-width: 990px) {
  .navbarTransparent{
    display: none;
  }

  .navbarCouleur{
    display: none;
  }
}
@media only screen and (max-width: 1550px) and (min-width: 991px){
  .navbarTransparent{
  background-color: rgba(172, 172, 172, 0.1);
  height: 4.5rem;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 23rem;
  position: fixed;
  width: 100%;
  z-index: 10;
}


.logo{
  width: 3.5rem;
  display: none;
}

.listeNavbar{
  display: flex;
  gap: 5rem
}

.membreListeNavbar{
  list-style-type: none;
  font-size: 1.2rem;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  color: #DFDFDF;
  cursor: pointer;
}

.social{
  display: none;
  gap: 2rem
}

.imageSocial{
  width: 1.5rem;
  opacity: 80%
}

      /* RESTE PAGE */

.navbarCouleur{
  transition: background-color 0.2s ease-in-out;
  background-color: var(--background-color);
  height: 4.5rem;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 23rem;
  position: fixed;
  width: 100%;
  box-shadow: 0px -2px 15px rgba(0, 0, 0, 0.25);
  z-index: 10;
}

.membreListeNavbarCouleur{
  list-style-type: none;
  font-size: 1.2rem;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  color: var(--font-color);
  cursor: pointer;
}
}
@media only screen and (min-width: 1551px){
  .navbarTransparent{
  background-color: rgba(172, 172, 172, 0.1);
  height: 4.5rem;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 23rem;
  position: fixed;
  width: 100%;
  z-index: 10;
}


.logo{
  width: 3.5rem;
}

.listeNavbar{
  display: flex;
  gap: 5rem
}

.membreListeNavbar{
  list-style-type: none;
  font-size: 1.2rem;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  color: #DFDFDF;
  cursor: pointer;
}

.social{
  display: flex;
  gap: 2rem
}

.imageSocial{
  width: 1.5rem;
  opacity: 80%
}

      /* RESTE PAGE */

.navbarCouleur{
  transition: background-color 0.2s ease-in-out;
  background-color: var(--background-color);
  height: 4.5rem;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 23rem;
  position: fixed;
  width: 100%;
  box-shadow: 0px -2px 15px rgba(0, 0, 0, 0.25);
  z-index: 10;
}

.membreListeNavbarCouleur{
  list-style-type: none;
  font-size: 1.2rem;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  color: var(--font-color);
  cursor: pointer;
}
}
        /*ACCUEIL*/



</style>