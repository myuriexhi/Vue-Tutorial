<template>
  <div>
    <p v-if="error.length">
        <b>please correct the following errors</b>
        <ul>
          <li v-for="e in error" v-bind:key="e.id">
            {{e}}
          </li>
        </ul>
    </p>
    <form @submit="login">
      <input type="text" placeholder="Enter Name" v-model="name" /><br /><br />
      <input
        type="password"
        placeholder="Enter Password"
        v-model="password"
      /><br /><br />
      <button type="Submit">Login</button>
    </form>
  </div>
</template>
<script>
export default {
  name: "Login1",
  data() {
    return {
      error: [],
      name: null,
      password: null,
    };
  },
  methods: {
    login(e) {
      this.error = [];
      if (this.name && this.password) {
        console.log("no error");
      }
      if (!this.name) {
        this.error.push("user name required");
      }
      if (!this.password) {
        this.error.push("password is  required");
      }
      console.log("hello", this.error);
      e.preventDefault();
    },
  },
};
</script>
