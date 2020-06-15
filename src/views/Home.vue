<template>
  <div class="home">
    <About/>
    <Portfolio/>
    <Contact/>
  </div>
</template>

<script>
// @ is an alias to /src
import About from "@/components/About.vue";
import Portfolio from "@/components/Portfolio.vue";
import Contact from "@/components/Contact.vue";

export default {
  name: "Home",
  components: {
    About,
    Portfolio,
    Contact
  }
};
</script>


<style scoped>
</style>