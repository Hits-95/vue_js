<template>
  <div>
    <h1>Hello HomeComponent</h1>
    <users />
    <Product />
    <Product />
  </div>
</template>
<script>
import Users from "./Users";
import Product from "./Product";

export default {
  name: "HomeComponent",
  components: {
    Users,
    Product,
  },
};
</script>
<style scoped>
div {
  background-color: #cbd7ec;
  height: 500px;
}
</style>