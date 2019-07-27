<template>
  <div class="container" id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>-->
    <Header />
    <hr />
    <ServerContainer />
    <Footer />
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
//import Home from "./components/Home.vue";
import Footer from "./components/Footer.vue";
import Header from "./components/Header.vue";
// import Servers from "./components/servers.vue";
// import ServerStatus from "./components/serverStatus.vue";
import ServerContainer from "./components/serverContainer.vue";
export default {
  name: "app",
  components: {
    Footer,
    Header,
    ServerContainer
  }
};
</script>

<style>
/* #app {
>>>>>>> 4f20f56edb6fae9814dcbfb3874b3f6dd261c02d
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>
