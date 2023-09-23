<template>
  <div id="app">
    <Header/>
    <Main/>
    <Footer/>
    <hr>
  </div>
</template>

<script>
import Header from "./components/header/Header.vue";
import Main from "./components/main/Main.vue";
import Footer from "./components/footer/Footer.vue";

export default {
  name: "app",
  components: {
    Footer: Footer,
    Main: Main,
    Header: Header,
  }
}
</script>

<style>
#app {
  background-color: #646cff;
}
</style>
