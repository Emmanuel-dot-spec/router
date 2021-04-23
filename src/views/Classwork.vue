<template>
  <div class="classwork">
    <form action="">
      <label for="name"></label>
      <input v-model="name" type="text" name="" placeholder="Enter your name" />
    </form>
    <div>
      <label for="email"></label>
      <input
        v-model="email"
        type="text"
        name=""
        placeholder="Enter your email"
      />
    </div>
    <button @click="submitform">Submit form</button>
  </div>
</template>

<script>
export default {
  name: "Classwork",
  data: () => {
    return {
      name: "",
      email: "",
    };
  },

  methods: {
    submitform() {
      alert(
        `welcome MR/MRS ${this.name} to our website, your email is ${this.email}`
      );
    },
  },
};
</script>

<style></style>
