<template>
  <div>
    <!-- <h1>Home1 Component</h1> -->
    <h1 class="Homestyle">Class and Style Binding</h1>
    <h1 v-bind:style="{ color: colorkey }">Style Binding</h1>
    <h1 v-bind:class="{ display: show, displayColor: show }">
      Class with object
    </h1>
    <h1 v-bind:class="[show ? 'yesShow' : 'NoShow']">Class With Array</h1>
    <!-- <p v-html="rowHtml"></p>
    <h3 v-once>{{ name }}</h3>
    <h3>{{ name }}</h3>
    <h3>{{ ok ? "yes" : "no" }}</h3>
    <button v-bind:Disabled="DisableBtn" v-on:click="UpdateText">
      Click Me
    </button> -->
    <!-- <Users />
    <Products /> -->
  </div>
</template>

<script>
//import Users from "./Users.vue";
//import Products from "./Products.vue";
export default {
  name: "Home1",
  data() {
    return {
      show: false,
      aclass: "classArray",
      colorkey: "red",
    };
  },
  //   data() {
  //     return {
  //       name: "mayuri",
  //       a: 10,
  //       b: 20,
  //       ok: true,
  //       rowHtml: "<h1>Template in vuejs</h1>",
  //       DisableBtn: false,
  //     };
  //   },
  //   methods: {
  //     UpdateText() {
  //       this.ok = !this.ok;
  //     },
  //   },
  //   components: {
  //     Users,
  //     Products,
  //   },
};
</script>
<style scoped>
.Homestyle {
  color: red;
}

.display {
  background-color: aquamarine;
}
.classArray {
  background-color: brown;
}
</style>
