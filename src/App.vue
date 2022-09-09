<template>
  <div id="app">
    <HelloWorld></HelloWorld>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'



export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data(){
    return{
      msg:'',
      profile:{}
    }
  },
mounted(){

    this.$liff.init({
    liffId: '1657453732-7J6wxlD9', // Use own liffId
})
console.log(this.$liff,'liff')
  },
  methods:{
   
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
