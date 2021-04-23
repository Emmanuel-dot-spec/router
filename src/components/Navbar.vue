<template>
  <div class="navbar">
    <nav>
      <p class="logo">En Masse</p>
      <div class="links">
        <!-- <a href="#">Home</a>
        <a href="#">Categories</a>
        <a href="#">FAQ</a>
        <a href="#">Become an Agent</a> -->
        <router-link :to="{ path: '/' }">Home</router-link>
        <router-link :to="{ path: '/categories' }">Categories</router-link>
        <router-link :to="{ path: '/faq' }">FAQ</router-link>
        <router-link :to="{ path: '/bag' }">Become an Agent</router-link>
      </div>
      <div class="buttons">
        <router-link :to="{ path: '/log-in' }"
          ><button class="sign-in">Sign In</button>
        </router-link>
        <router-link :to="{ path: '/sign-up' }"
          ><button class="sign-up">Sign Up</button></router-link
        >
      </div>
    </nav>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: #ffffff;
  padding: 0 50px;
  box-shadow: 0px 3px 10px rgba(0, 0, 0, 0.1);
}
.links a {
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
  line-height: 19px;
  color: #4f4f4f;
  margin-left: 10px;
  text-decoration: none;
}
.buttons .sign-in {
  font-weight: 500;
  font-size: 18px;
  line-height: 22px;
  color: #363154;
  background: none;
  border: none;
  cursor: pointer;
}
.buttons .sign-up {
  background: #ffa010;
  border-radius: 1px solid #ffa010;
  border-radius: 8px;
  margin-left: 20px;
  padding: 10px 20px;
  cursor: pointer;
}
</style>
