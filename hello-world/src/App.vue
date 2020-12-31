<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <!-- <Home data="Hitesh Ahire" msg="done" /> -->
    <!-- <Forloop /> -->
    <!-- <HomeComponent /> -->
    <!-- <Template /> -->
    <!-- <Class1 /> -->
    <!-- <DataBind /> -->
    <Props />
  </div>
</template>

<script>
// import Forloop from "./components/Forloop.vue";
// import HelloWorld from './components/HelloWorld.vue'
// import Home from "./components/Home.vue";
// import HomeComponent from "./components/HomeComponent.vue";
// import Template from "./components/Template.vue";
// import Class1 from "./components/Class1.vue";
// import DataBind from "./components/DataBind";
import Props from "./components/Props.vue";

export default {
  name: "App",
  components: {
    //HelloWorld,
    // Home,
    // Forloop,
    // HomeComponent,
    // Template,
    // Class1,
    // DataBind,
    Props,
  },
};
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
