<template>
  <div id="app">
    <Navbar class="navbar" />
    <router-view />
    <Footer />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";

export default {
  components: {
    Navbar,
    Footer
  },
  data() {
    return {};
  }
};
</script>

<style>
#app {
  font-family: "Montserrat", sans-serif;
  scroll-behavior: smooth;
}
/* .navbar {
  margin: 0 0 3rem 0;
} */
</style>
