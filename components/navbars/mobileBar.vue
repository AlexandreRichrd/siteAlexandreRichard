<template>
  <header :id="$style['mobile-bar']">
    <img src="../../static/images/burger.svg" :class="$style['image-burger']" alt="un burger" @click="toogleNav()">
    <ul :class="nav ? $style['links-toogled'] : $style['links-untoogled']">
      <li>Accueil</li>
      <li>A propos</li>
      <li>Competences</li>
      <li>Portfolio</li>
    </ul>

  </header>
</template>

<script>
export default {
  data(){
    return{
      nav: false
    }
  },
  methods: {
    toogleNav(){
      this.nav = !this.nav
    }
  }
}
</script>

<style module>
@media only screen and (max-width: 990px) {
  #mobile-bar{
  }

  .image-burger{
    position: absolute;
    cursor: pointer;
    z-index: 11;
    margin: 1rem;
  }

  .links-toogled{
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: #696969b6;
    height: 84%;
    position: absolute;
    z-index: 10;
    transform: translateY(0);
    transition: transform 0.2s ease-in-out;
    padding: 8rem 0 0 0;
    width: 100%;
  }

  .links-toogled li{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 8rem;

    list-style-type: none;
    font-size: 1.6rem;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;


    border-bottom: 1px solid rgb(105, 105, 105);

    cursor: pointer;
  }

  ul{
    margin: 0;
  }

  .links-untoogled{
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: #696969b6;
    height: 100vh;
    position: absolute;
    z-index: 10;
    transform: translateY(-120vh);
    transition: transform 0.2s ease-in-out;
    padding: 8rem 0 0 0;
    width: 100%;
  }

  .links-untoogled li{
    list-style-type: none;
    font-size: 1.6rem;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    border-bottom: 1px solid rgb(105, 105, 105);
  }
}
@media only screen and (min-width: 991px){
  #mobile-bar{
    display: none;
  }

  .image-burger{
    display:none;
  }

  .links-untoogled{
    display: none;
  }

  .links-toogled{
    display: none;
  }

}
</style>