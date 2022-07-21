<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <test msg="lzp" @tap1="tap"></test>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import test from './components/test.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    test
  },
  methods:{
      tap:function(e){
          console.log(e);
      }
  }
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
