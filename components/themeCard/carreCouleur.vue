<template>
  <div :class="$style['carre']" :style="{'background-color': '#' + couleurhexa}" @click="toogleMainColor()">

  </div>
</template>

<script>
  export default {
    props: {
      couleurhexa: {
        type: String,
        required: true
      },
      couleur: {
        type: String,
        required: true
      }
    },
    methods: {
      toogleMainColor(){
        console.log(this.couleur)
        document.documentElement.setAttribute('main-color', this.couleur);
      }
    }
    
  }
</script>

<style module>
.carre{
width: 2.5rem;
height: 2.5rem;
cursor: pointer;
}
</style>