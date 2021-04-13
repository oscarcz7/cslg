<template>
  <div id="app">
    <Nav />
    <div >
      <router-view />
    </div>
    <Footer />
  </div>
</template>
<script>
import Footer from "./components/partials/Footer.vue";
import Nav from "./components/partials/Nav.vue";
export default {
  name: "app",
  components: {
    Nav,
    Footer,
  },
};
</script>
<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>