<template>
  <div class="faq">
    <Navbar />
    <h1>FAQ Page</h1>
    <Footer />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
export default {
  name: "Faq",
  components: {
    Navbar,
    Footer,
  },
};
</script>

<style scoped></style>
