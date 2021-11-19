<template>
  <div>
    <input
      type="text"
      placeholder="Enter Your Name"
      v-model="signup.username"
    /><br /><br />
    <input
      type="text"
      placeholder="Enter Your password"
      v-model="signup.password"
    /><br /><br />

    <p>Choose Hobbies</p>
    <input
      type="checkbox"
      id="cricket"
      value="cricket"
      v-model="signup.hobbies"
    />
    <label for="cricket"> Cricket</label>
    <input
      type="checkbox"
      id="Football"
      value="Football"
      v-model="signup.hobbies"
    />
    <label for="Football">Football</label><br />
    <p>Choose Gender</p>
    <input type="radio" id="Female" value="Female" v-model="signup.gender" />
    <label for="Female"> Female</label>
    <input type="radio" id="Male" value="Male" v-model="signup.gender" />
    <label for="Male">Male</label><br /><br />
    <button v-on:click="signUpUsers">SignUp</button>
  </div>
</template>
<script>
export default {
  name: "SignUp",
  data() {
    return {
      signup: {
        username: null,
        password: null,
        hobbies: [],
        gender: null,
      },
    };
  },

  methods: {
    signUpUsers() {
      console.log(this.signup);
    },
  },
};
</script>
