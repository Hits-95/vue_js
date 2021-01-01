<template>
  <div>
    <h1>{{ msg }}</h1>
    Name :
    <input
      type="text"
      placeholder="Enter your name"
      v-model="sign_up.username"
    />
    <br /><br />
    password :
    <input
      type="password"
      placeholder="Enter your password"
      v-model="sign_up.password"
    />
    <br /><br />
    <p>chose hobbies</p>
    <input type="checkbox" id="game" value="game" v-model="sign_up.hobbies" />
    <label for="game"> Game </label>
    <input type="checkbox" id="study" value="study" v-model="sign_up.hobbies" />
    <label for="study"> Game </label>
    <br /><br />
    <p>chose gender</p>
    <input type="radio" id="male" value="male" v-model="sign_up.gender" />
    <label for="male">Male </label>
    <input type="radio" id="female" value="female" v-model="sign_up.gender" />
    <label for="female"> Female </label>
    <br /><br />
    <button v-on:click="signupUser">Sign_up</button>
  </div>
</template>

<script>
export default {
  name: "Check_Radio",
  data() {
    return {
      msg: "Check_Radio",
      sign_up: {
        username: null,
        password: null,
        hobbies: [],
        gender: null,
      },
    };
  },
  methods: {
    signupUser() {
      console.warn(this.sign_up);
    },
  },
};
</script>

<style scoped>
</style>