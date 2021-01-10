<template>
  <div>
    <h1>{{ msg }}</h1>
    <p v-if="validation.error">
        <b>correct the errors</b>
        <ul>
            <li v-for="e in validation.error" v-bind:key="e.id">
                    {{e}}
            </li>
        </ul>
    </p>
    <form @submit="login">
      <input
        type="text"
        placeholder="Enter username"
        v-model="validation.name"
      /><br /><br />
      <input
        type="password"
        placeholder="Enter password"
        v-model="validation.password"
      /><br /><br />
      <button type="submit">Login</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "Login_validation",

  data() {
    return {
      msg: "Login Form Validation",
      validation: {
        error: [],
        name: null,
        password: null,
      },
    };
  },

  methods: {
    login(event) {
      this.error = [];
      if (this.validation.name && this.validation.password) {
        console.log("no error");
      }
      if (!this.validation.name) {
        console.log("ho");
        this.validation.error.push("user name is requerd");
      }
      if (!this.validation.password) {
        console.log("qqq1");
        this.validation.error.push("password is requerd");
      }
      console.warn("done", this.validation.error);
      event.preventDefault();
    },
  },
};
</script>

<style scoped>
</style>