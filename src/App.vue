<template>
  <div id="app">
<!--    <img alt="Vue logo" src="./assets/logo.png">-->
<!--    <HelloWorld msg="Welcome to Your Vue.js App"/>-->
<!--    <Home data="Home Data" msg="Hi From message"></Home>-->
    <Home></Home>
    <users></users>
    <product></product>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue';
import Home from "./components/Home";
import Users from "./components/Users";
import Product from "./components/Products";
export default {
  name: 'App',
  components: {
    Home,
    Users,
    Product
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
