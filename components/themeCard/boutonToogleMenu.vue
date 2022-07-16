<template>
  <div :class="scroll ? $style['bouton'] : $style['depart']">
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

        if(window.scrollY <= 610){
          this.scroll = false
        }else{
          this.scroll = true
        }
        console.log(window.scrollY)
      })
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
  animation: display 3s ease-in-out;
  justify-content: center;
  align-items: center;
  /* position: absolute;
  top: 50%; */
  left: 28.5rem;
}

.depart{
  animation: display 3s ease-in-out;
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