<template>
  <div>
    <h1>For Loop in vue js...</h1>
    <table border="1px">
      <tr>
        <th>ID</th>
        <th>Name</th>
        <th>Email</th>
      </tr>
      <tr v-for="user in users" :key="user.id">
        <th>{{ user.id }}</th>
        <th>{{ user.name }}</th>
        <th>{{ user.email }}</th>
      </tr>
    </table>
  </div>

  <!-- <h2>{{data}}</h2>
		<h2>{{msg}}</h2> -->
</template>
<script>
export default {
  name: "Forloop",
  props: {
    data: String,
    msg: String,
  },
  data() {
    return {
      users: [
        { id: 1, name: "hitesh1", email: "hbahire1@gmail.com" },
        { id: 2, name: "hitesh2", email: "hbahire2@gmail.com" },
        { id: 3, name: "hitesh3", email: "hbahire3@gmail.com" },
      ],
    };
  },
};
</script>