<template>
  <div>
    <!-- <h1>{{ name | Ucase }}</h1> -->
    <h1>{{ name }}</h1>
  </div>
</template>
<script>
export default {
  name: "Home2",
  //   data() {
  //     return {
  //       name: "Home2",
  //     };
  //   },
  data() {
    return {
      name: "mayuri patel",
    };
  },
  //   created() {
  //     console.log("created", this.name);
  //   },
  //   beforeCreate() {
  //     this.name = "pratik";
  //     console.log("before", this.name);
  //   },

  beforeMount() {
    console.log("beforeMount", this.$el);
  },

  mounted() {
    console.log("mounted", this.$el);
  },
};
</script>
