<template>
  <div class="row">
    <h1><b>Edit Form</b></h1>
    <center>
      <b>First Name:</b>
      <input
        type="text"
        v-model="user.firstName"
        :disabled="!isEditing"
        :class="{ view: !isEditing }"
      /><br /><br />
      <b>Last Name:</b>
      <input
        type="text"
        v-model="user.lastName"
        :disabled="!isEditing"
        :class="{ view: !isEditing }"
      /><br /><br />
      <center>
        <button @click="isEditing = !isEditing">
          {{ isEditing ? "Save" : "Edit" }}</button
        >&nbsp;
        <button v-if="isEditing" @click="isEditing = false">Cancel</button>
      </center>
    </center>
  </div>
</template>

<script>
export default {
  name: "EditForm",
  data() {
    return {
      isEditing: false,
      user: {
        firstName: "mayuri",
        lastName: "patel",
      },
    };
  },
};
</script>

<style>
.view {
  border-color: transparent;
  background-color: initial;
  color: initial;
}
.row {
  background-color: rgb(241, 191, 191);
  margin-left: 700px;
  margin-right: 700px;
}
</style>
