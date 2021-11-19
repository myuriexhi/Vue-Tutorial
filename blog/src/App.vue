<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
    <!--<HelloWorld msg="Welcome to Your Vue.js App" />-->
    <!-- <Home data="Mayuri Is Here" msg="Hi from Mayuri" /> -->
    <!-- <Home1 /> -->
    <!-- <h1>Data Binding In Vuejs</h1>
    <DataBind /> -->
    <!-- <h1>Props In Vuejs</h1>
    <Child v-bind:users="users" /> -->

    <!-- <h1>{{ title }}</h1>
    <Child1 v-on:changetitle="updatetitle($event)" /> -->
    <!-- <h1>SignUp Form</h1>
    <SignUp /> -->
    <!-- <h1>Login Form</h1>
    <Login /> -->
    <!-- <h1>VALIDATION FORM</h1>
    <Login1 /> -->
    <!-- <h1>Filter In Vue</h1>
    {{ name | Ucase }}
    <Home2 /> -->
    <!-- <h1>beforeCreate and created lifecycle hooks</h1>
    <Home2 /> -->

    <EditForm />
  </div>
</template>

<script>
//import HelloWorld from "./components/HelloWorld.vue";
//import Home from "./components/Home.vue";
//import Home1 from "./components/Home1.vue";
//import DataBind from "./components/DataBind.vue";
//import Child from "./components/Child.vue";
//import Child1 from "./components/Child1.vue";
//import SignUp from "./components/SignUp.vue";
//import Login from "./components/Login.vue";
//import Login1 from "./components/Login1.vue";
//import Home2 from "./components/Home2.vue";
import EditForm from "./components/EditForm.vue";

export default {
  name: "App",
  components: {
    // HelloWorld,
    //Home,
    //Home1,
    //DataBind,
    //Child,
    //Child1,
    //SignUp,
    //Login,
    //Login1,
    // Home2,
    EditForm,
  },
  // data() {
  //   return {
  //     name: "mayuri patel",
  //   };
  // },
  // data() {
  //   return { title: "props tutorial" };
  // },
  // methods: {
  //   updatetitle(title) {
  //     this.title = title;
  //   },
  // },
  // data() {
  //   return {
  //     users: [
  //       { name: "Mitu", email: "mitu@test.com" },
  //       { name: " Mitu", email: "mitu@test.com" },
  //       { name: "Mitu ", email: "mitu@test.com" },
  //       { name: "Mitu ", email: "mitu@test.com" },
  //     ],
  //   };
  // },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
