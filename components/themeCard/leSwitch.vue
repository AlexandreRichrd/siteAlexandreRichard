<template>
  <div :class="dark ? $style['switch1'] : $style['switch2']" @click="toogleTheme()">
    <div :class="dark ? $style['boutonSwitch2'] : $style['boutonSwitch1']" />
  </div>
</template>

<script>
export default {
  data(){
    return{
      dark: false
    }
  },
  methods:{
    toogleTheme(){
      this.dark = !this.dark
      if(this.dark){
        document.documentElement.setAttribute('data-theme', 'darkMode');
      }else{
        document.documentElement.setAttribute('data-theme', '');
      }
        
    }
  }
}
</script>

<style module>
.switch1{
  background-color: #969696;
  width: 4.3rem;
  height: 2.5rem;
  border-radius: 30px;
  display: flex;
  align-items: center;
  padding: 0 0.2rem;
  cursor: pointer;
}

.switch2{
  background-color: #969696;
  width: 4.3rem;
  height: 2.5rem;
  border-radius: 30px;
  display: flex;
  align-items: center;
  padding: 0 0.2rem;
  cursor: pointer;
}

.boutonSwitch1{
  background-image: url("@/static/images/light.png");
  background-size: cover;
  border-radius: 50%;
  height: 2rem;
  width: 2rem;
  transition: all 0.5s ease-in-out;
}

.boutonSwitch2{
  background-image: url("@/static/images/dark.png");
  background-size: cover;
  border-radius: 50%;
  height: 2rem;
  width: 2rem;
  float: right;
  margin-left: 2.2rem;
  transition: all 0.5s ease-in-out;
}
</style>