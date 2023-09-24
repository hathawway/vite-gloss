<template>
  <div id="main">
    <ListWord/>
  </div>
</template>

<script>
import ListWord from "./ListWord.vue";

export default {
  name: "main",
  components: {
    ListWord: ListWord,
  }
}
</script>

<style>
#main {
  background-color: #fff;
  padding: 30px;
}
</style>