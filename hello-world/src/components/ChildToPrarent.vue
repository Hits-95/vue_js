// send child to parent

<template>
  <div>
    <h1>ChildToPrarent Props Component</h1>
    <button v-on:click="UpdateTitle">Update Prarent Title</button>
  </div>
</template>

<script>
export default {
  name: "ChildToPrarent",
  methods: {
    UpdateTitle() {
      this.$emit("changeTitle", "Parent Updated....");
    },
  },
};
</script>

<style scoped>
</style>