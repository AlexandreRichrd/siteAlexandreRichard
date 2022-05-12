<template>
  <div :class="scroll ? $style['bouton'] : $style['depart']" @mouseenter="toogleMenu()" @mouseleave="untoogleMenu()">
    <img src="@/static/images/settings.png" alt="">
  </div>
</template>

<script>
  export default {
    data(){
      return{
        scroll: false,
        hover: false
      }
    },
    mounted(){
      document.addEventListener("scroll", () => {

        if(window.scrollY <= 570){
          this.scroll = false
        }else{
          this.scroll = true
        }
      })
    },
    methods: {
      toogleMenu(){
        this.hover = true
        this.$emit('souris-dessus', this.hover)
      },
      untoogleMenu(){
        this.hover = false
        this.$emit('souris-dessus', this.hover)
      }
    }
  }
</script>

<style module>
.bouton{
  border-radius: 0 20px 20px 0;
  height: 12rem;
  width: 5rem;
  background-color: rgb(202, 202, 202);
  display: flex;
  justify-content: center;
  align-items: center;
  position: fixed;
  top: 50%;
  left: 28.5rem;
}

.depart{
  display: none;
}

.bouton img{
  width: 3rem;
}

.bouton img:hover{
  animation: rotation 2s infinite linear;
}

@keyframes rotation {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(359deg);
  }
}
</style>