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
};
</script>
