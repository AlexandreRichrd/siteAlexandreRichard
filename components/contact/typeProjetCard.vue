<template>
  <div :class="$style['cardProjet']">
    <img src="@/static/images/linternet.png" alt="">
    <h6>{{ cardName }}</h6>
  </div>
</template>

<script>
  export default {
    props: {
      cardName: {
        type: String,
        required: true
      }
    }
  }
</script>

<style module>
.cardProjet{
  background-color: var(--background-color);
  width: 6rem;
  height: 6rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  border-radius: 12px;
  box-shadow: 2px 2px 4px rgba(0, 0, 0, 0.25);
  cursor: pointer;
}

.cardProjet img{
  width: 3.9rem;
  height: 3.9rem;
}

.cardProjet h6{
  text-transform: uppercase;
  color: #8A8A8A;
  font-weight: 400;
  margin: 0;
}

.cardProjet:hover{
  box-shadow: 1x 1px 4px rgb(79, 79, 79);
}
</style>