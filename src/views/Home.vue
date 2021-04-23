<template>
  <div class="home">
    <Navbar />
    <router-link :to="{ name: 'dashboard' }">Go to Dashboard</router-link>
    <h1>Home Page</h1>
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "Home",
  components: {
    Navbar,
    Footer,
  },
};
</script>
