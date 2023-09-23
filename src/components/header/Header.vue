<template>
  <div id="header">
    <Search/>
    <hr>
  </div>
</template>

<script>
import Search from "./search/Search.vue";

export default {
  name: "header",
  components: {
    Search: Search,
  }
}
</script>

<style>

</style>