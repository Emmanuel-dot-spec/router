<template>
  <div class="sign-up">
    <Navbar />
    <div class="body">
      <div class="heading">
        <h2>Sign Up For An Account</h2>
        <p>
          We’ll like to meet you please fill in your name, email, phone number
          and password
        </p>
      </div>
      <form class="form">
        <div class="form-group">
          <label for="Fullname" class="label">Fullname</label>
          <input class="input" type="text" placeholder="Olagoke Olawuni" />
        </div>
        <div class="form-group">
          <label for="Email" class="label">Email</label>
          <input class="input" type="text" placeholder="gokr@email.com" />
        </div>
        <div class="form-group">
          <label for="Phone" class="label">Phone Number</label>
          <input class="input" type="number" placeholder="012345678" />
        </div>
        <div class="form-group">
          <label for="Password" class="label">Password</label>
          <input class="input" type="text" placeholder="password" />
        </div>
        <button class="register-button">Register</button>
        <p class="under-register">
          Already have an account?<span class="under-register2">Log In</span>
        </p>
      </form>
    </div>
    <Footer />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "Signup",
  components: {
    Navbar,
    Footer,
  },
};
</script>

<style scoped>
.heading {
  text-align: center;
}
.heading h2 {
  font-style: normal;
  font-weight: bold;
  font-size: 36px;
  line-height: 44px;
  color: #03363c;
}
.heading p {
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  line-height: 22px;
  color: #3e3e3e;
}
.form {
  max-width: 400px;
  display: block;
  margin: auto;
}
.form-group {
  display: flex;
  flex-direction: column;
  margin-top: 20px;
}
.form-group .label {
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 20px;
  color: #3e3e3e;
  padding-left: 12px;
}
.form-group .input {
  background: #ffffff;
  border: 1px solid #dfdfdf;
  box-sizing: border-box;
  border-radius: 7px;
  height: 50px;
  padding: 10px 10px;
  margin: 10px;
}
.register-button {
  background: #ffa010;
  border: 1px solid #ffa010;
  box-sizing: border-box;
  box-shadow: 0px 4px 10px rgba(24, 116, 191, 0.15);
  border-radius: 7px;
  height: 50px;
  margin-top: 35px;
  width: 100%;
  font-style: normal;
  /* text style */
  font-weight: bold;
  font-size: 16px;
  line-height: 29px;
  letter-spacing: -0.04em;
  color: #f7f7f7;
}
.under-register {
  text-align: center;
  margin: 24px 0 62px 0;
}
.under-register2 {
  font-family: Mulish;
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 20px;
  color: #2e9eb6;
}
</style>
