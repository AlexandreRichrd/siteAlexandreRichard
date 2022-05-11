<template>
  <div :class="$style['bouton']">
    <img src="@/static/images/settings.png" alt="">
  </div>
</template>

<script>
  export default {

  }
</script>

<style module>
.bouton{
  border-radius: 0 20px 20px 0;
  height: 11rem;
  width: 5rem;
  background-color: rgb(202, 202, 202);
  display: flex;
  justify-content: center;
  align-items: center;
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