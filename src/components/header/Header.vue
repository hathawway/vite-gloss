<template>
  <div class="header-search">
    <Search/>
    </div>
</template>

<script>
import Search from "./search/Search.vue";

export default {
  name: "HeaderComponent",
  components: {
    Search: Search,
  }
}
</script>

<style>
.header-search {
  padding: 20px 0px;
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}

</style>
