<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->

    <!-- Detta tar emot helloworld komponenten -->
    <!-- msg skickar meddelandet till helloworld component -->
    <HelloWorld msg="Welcome to Your Vue.js App"/>

    <value/>
    <colorMode/>
    <showOrHide/>

  </div>
</template>

<script>
// Tar emot hello world komponenten
import HelloWorld from './components/HelloWorld.vue'
import value from './components/value.vue'
import colorMode from './components/colorMode.vue'
import showOrHide from './components/showOrHide.vue'


//Tar emot Hello World komponenten
export default {
  name: 'App',
  components: {
    HelloWorld,
    value,
    colorMode,
    showOrHide
  }
}
</script>

<style>
*{
  box-sizing:border-box;
  margin:0;
  padding:0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
   background-color:rgb(134, 119, 150);
  /* margin-top: 60px; */
  
}
</style>
