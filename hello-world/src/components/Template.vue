<template>
  <div>
    <p v-html="user.rowHtml"></p>
    <h2 v-once>{{ user }}</h2>
    <h2>{{ user }}</h2>
    <h3>{{ user.ok ? "Yess" : "Nooo" }}</h3>
    <button v-bind:disabled="user.disableBtn" v-on:click="updateText">
      {{ user.ok ? "true" : "False" }}
    </button>
  </div>
</template>
<script>
export default {
  name: "Template",
  data() {
    return {
      user: {
        id: 2,
        name: "Ervin Howell",
        username: "Antonette",
        email: "Shanna@melissa.tv",
        ok: false,
        rowHtml: "<h1>Template Component</h1>",
        disableBtn: false,
      },
    };
  },
  methods: {
    updateText() {
      this.user.name = "Hitesh Ahire";
      this.user.ok = !this.user.ok;
    },
  },
};
</script>
<style scoped>
</style>