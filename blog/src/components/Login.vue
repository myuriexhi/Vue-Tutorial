<template>
  <div>
    <input
      type="text"
      Name="username"
      v-model="LoginForm.username"
      placeholder="Enter Your name"
    /><br /><br />
    <input
      type="password"
      Name="password"
      v-model="LoginForm.password"
      placeholder="Enter your Password"
    /><br /><br />
    <button v-on:click="loginData">Login</button>
  </div>
</template>
<script>
export default {
  name: "Login",

  methods: {
    loginData() {
      console.log(
        "loginData",
        this.LoginForm.username,
        this.LoginForm.password
      );
    },
  },
  data() {
    return {
      LoginForm: { username: null, password: null },
    };
  },
};
</script>
