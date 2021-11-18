<template>
  <div>
    <button v-on:click="updatetitle">Update Parent Title</button>
  </div>
</template>
<script>
export default {
  name: "Child",
  methods: {
    updatetitle() {
      this.$emit("changetitle", "parent updated");
    },
  },

  beforeMount: function () {
    console.log("beforeMount");
  },
  mounted: function () {
    console.log("mounted");
  },
  created: function () {
    console.log("created");
  },
  beforeCreate: function () {
    console.log("beforecreated");
  },
};
</script>
