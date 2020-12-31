<template>
  <div>
    <h1 class="homestyle">Class1 Component</h1>
    <h2 v-bind:style="{ color: 'blue' }">style binding</h2>
    <h3 v-bind:class="{ display: show, displayColor: show }">
      Class binging with object
    </h3>
    <h4 v-bind:class="[show ? 'displayColor' : 'display']">
      Class binging with object
    </h4>
  </div>
</template>

<script>
export default {
  name: "Class1",
  data() {
    return {
      show: true,
    };
  },
};
</script>

<style scoped>
.homestyle {
  color: #ec2d2d;
}
.display {
  background-color: palegreen;
}
.displayColor {
  color: #f30505;
}
</style>