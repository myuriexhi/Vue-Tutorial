<template>
  <div>
    <!-- <h1>Hello From Home Component</h1> -->
    <h1>For Loop vuejs</h1>
    <!-- <h1 v-if="show">Conditional Rendering vuejs</h1>
    <h1 v-else>Conditional Rendering else block</h1>
    <button v-on:click="display">Toggle Elements</button> -->
    <!-- <h2>{{ data }}</h2>
    <h2>{{ msg }}</h2> -->
    <!-- <button v-on:mouseover="Hello('HELLO FUNCTION')">
      Hello function call
    </button> -->
    <table border="1px">
      <tr>
        <td>Id</td>
        <td>Name</td>
        <td>Email</td>
      </tr>

      <tr v-for="user in users" :key="user.id">
        <td>{{ user.id }}</td>
        <td>{{ user.name }}</td>
        <td>{{ user.email }}</td>
      </tr>
    </table>
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
    return {
      users: [
        { id: 1, name: "Mayu", email: "mayu@test.com" },
        { id: 2, name: "piku", email: "piku@test.com" },
        { id: 3, name: "resu", email: "resu@test.com" },
        { id: 4, name: "pratik", email: "pk@test.com" },
      ],
    };
  },

  //   data() {
  //     return { show: true };
  //   },
  //   methods: {
  //     display() {
  //       this.show = !this.show;
  //     },
  //   },
  //   methods: {
  //     Hello(data) {
  //       alert(data);
  //     },
  //   },
};
</script>
