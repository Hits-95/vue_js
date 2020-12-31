<template>
  <div>
    <h1>Data Bind</h1>
    <h2>{{ msg }}</h2>
    <input type="text" v-model="msg" />
  </div>
</template>
<script>
export default {
  name: "DataBind",
  data() {
    return { msg: "Enter value" };
  },
};
</script>