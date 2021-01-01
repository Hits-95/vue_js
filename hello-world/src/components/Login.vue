<template>
  <div>
    <h1>{{ msg }}</h1>
    Username :
    <input
      type="text"
      placeholder="Enter username"
      v-model="loginForm.username"
    />
    <br /><br />
    Password :
    <input
      type="password"
      placeholder="Enter password"
      v-model="loginForm.password"
    /><br /><br />
    <button v-on:click="loginData">Login</button>
  </div>
</template>

<script>
export default {
  name: "Login",
  data() {
    return {
      msg: "Login Form",
      loginForm: {
        username: null,
        password: null,
      },
    };
  },
  methods: {
    loginData() {
      console.log(
        "loginData",
        this.loginForm.username,
        this.loginForm.password
      );
    },
  },
};
</script>

<style scoped>
</style>