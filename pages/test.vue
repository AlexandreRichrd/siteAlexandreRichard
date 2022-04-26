<template>
  <div :class="etat ? $style['goodbye'] : $style['hello']">
    <button @click="test()">test</button>
    sheesh
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data(){
    return{
      etat: false
    }
  },
  methods: {
    test(){
      this.etat = true;
      console.log(this.etat);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style module>
.hello{
  height: 100px;
  background-color: blueviolet;
}

.goodbye{
  height: 100px;
  background-color: red;
}
</style>
