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
    <!-- <Props v-bind:users="users" /> -->
    <!-- <h1>{{ title }}</h1>
    <ChildToPrarent v-on:changeTitle="UpdateTitle($event)" /> -->
    <!-- <Check_Radio /> -->
    <!-- <Form_getData /> -->
    <!-- <Login /> -->
    <!-- <Login_validation /> -->
    <Filter_form />
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
// import Props from "./components/Props.vue";
// import ChildToPrarent from "./components/ChildToPrarent.vue";
// import Check_Radio from "./components/Check_Radio.vue";
// import Form_getData from "./components/Form_getData.vue";
// import Login from "./components/Login.vue";
// import Login_validation from "./components/Login_validation";
import Filter_form from "./components/Filter_form.vue";

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
    // Props,
    // ChildToPrarent,
    // Check_Radio,
    // Form_getData,
    // Login,
    // Login_validation,
    Filter_form,
  },
  // data() {
  //   return {
  //     title: "Send Props child to Prarent",
  //   };
  // return {
  //   users: [
  //     { name: "Hitesh", email: "hbasfsdfsdf" },
  //     { name: "PD", email: "hbasfsdfsdf" },
  //     { name: "Nikita", email: "hbasfsdfsdf" },
  //   ],
  // };
  // methods: {
  //   UpdateTitle(title) {
  //     this.title = title;
  //   },
  // },
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
