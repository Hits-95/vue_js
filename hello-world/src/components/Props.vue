// SEND DATA PRARENT TO CHILED

<template>
  <div>
    <h1>Props Component</h1>
    <h2 v-for="user in users" :key="user.name">
      {{ user.name }} = {{ user.email }}
    </h2>
  </div>
</template>

<script>
export default {
  name: "Props",
  props: ["users"],
};
</script>

<style scoped>
</style>