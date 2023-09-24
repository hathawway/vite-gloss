<template>
    <Header/>
    <Main/>
    <Footer/>
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
</style>
