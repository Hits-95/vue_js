<template>
  <div>
    <h1>Hello HomeComponent</h1>
    <users />
  </div>
</template>
<script>
import Users from "./Users";

export default {
  name: "HomeComponent",
  components: {
    Users,
  },
};
</script>
<style scoped>
div {
  background-color: #cbd7ec;
  height: 500px;
}
</style>