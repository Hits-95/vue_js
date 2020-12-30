<template>
  <div>
    <h1 v-if="show">Hellow online...</h1>
    <!-- <h2>{{data}}</h2>
		<h2>{{msg}}</h2> -->

    <div v-else>
      <button v-on:click="hello('hitesh Ahire')">click</button>
      <button v-on:mouseover="hello('hitesh Ahire')">mouseover</button>
      <button v-on:mouseout="hello('hitesh Ahire')">mouseout</button>
    </div>
    <button v-on:click="display">Toggle</button>
  </div>
</template>
<script>
export default {
  name: "Home",
  props: {
    data: String,
    msg: String,
  },
  data() {
    return { show: true };
  },
  methods: {
    display() {
      this.show = !this.show;
      //   console.log(this.show);
    },
    hello(data) {
      //   console.log("Home.vue console");
      alert(data);
    },
  },
};
</script>