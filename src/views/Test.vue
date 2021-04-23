<template>
  <div class="test">
    <p>{{ name }}</p>
    <form action="">
      <label for="name"></label>
      <input v-model="name" type="text" placeholder="Enter your name" />
    </form>
    <p>{{ email }}</p>
    <form action="">
      <label for="email"></label>
      <input v-model="email" type="text" placeholder="Enter your email" />
    </form>
    <button @click="submit">Submit</button>
  </div>
</template>

<script>
export default {
  name: "Test",
  data: () => {
    return {
      name: "",
      email: "",
    };
  },
  methods: {
    submit() {
      alert(
        `welcome Mr/Mrs ${this.name} to our website, your email is ${this.email}`
      );
    },
  },
};
</script>

<style></style>
