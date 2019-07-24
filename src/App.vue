<template>
  <div class="container" id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>-->
    <Header/>
    <hr>
    <ServerStatus/>
    <Footer/>
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
//import Home from "./components/Home.vue";
import Footer from "./components/Footer.vue";
import Header from "./components/Header.vue";
import ServerStatus from "./components/ServerStatus.vue";
export default {
  name: "app",
  components: {
    Footer,
    Header,
    ServerStatus
  }
};
</script>

<style>
/* #app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>
