<template>
  <div class="populate-table">
    <form>
      <div class="form_item">
        <label for="name">Full Name</label>
        <input type="text" name="name" v-model="newUser.fullName" />
      </div>
      <div class="form_item">
        <label for="email">Email Address</label>
        <input type="text" v-model="newUser.email" />
      </div>
      <div class="form_item">
        <label for="phone">Phone Number</label>
        <input type="text" name="phone" id="phone" v-model="newUser.phone" />
      </div>
      <button @click.prevent="submitForm" :disabled="checkIfFormIsComplete">
        Send
      </button>
    </form>
    <div>
      <table>
        <thead>
          <tr>
            <th>Full Name</th>
            <th>Email Address</th>
            <th>Phone Number</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="user in allUsers" v-bind:key="user.id">
            <td>{{ user.fullName }}</td>
            <td>{{ user.email }}</td>
            <td>{{ user.phone }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>
export default {
  name: "PopulateTable",
  data: () => {
    return {
      newUser: {
        fullName: "",
        email: "",
        phone: "",
      },
      allUsers: [],
    };
  },
  computed: {
    checkIfFormIsComplete() {
      return (
        !this.newUser.fullName && !this.newUser.email && !this.newUser.phone
      );
    },
  },
  methods: {
    submitForm() {
      alert("Submission Successful");
      this.allUsers.push(this.newUser);
      this.clearForm();
    },
    clearForm() {
      this.newUser = {
        fullName: "",
        email: "",
        phone: "",
      };
    },
  },
};
</script>

<style scoped>
form {
  max-width: 400px;
  background: coral;
  padding: 2rem;
  border-radius: 8px;
  margin: 40px auto;
}
.form_item {
  display: block;
  max-width: 100%;
  margin-bottom: 1rem;
}
.form_item > label {
  display: block;
}
.form_item > input {
  padding: 1rem;
  font-size: 18px;
  border-radius: 8px;
  color: coral;
  background: #fff;
  border: 2px solid coral;
  width: 90%;
}
button {
  padding: 1rem 3rem;
  background: black;
  color: #fff;
  cursor: pointer;
}
button:disabled,
button[disabled] {
  cursor: not-allowed;
}
table {
  border: 1px solid black;
  width: 100%;
}
td,
th {
  border: 1px solid #3333;
  padding: 1rem;
}
tr:nth-child(even) {
  background: #dbdbdb;
}
</style>
