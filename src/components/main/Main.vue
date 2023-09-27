<template>
  <div class="main-words">
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
.main-words {
  flex: 1 0 auto;

  background-color: rgba(255, 255, 255, 0.98);
  border-top-right-radius: 30px;
  border-top-left-radius: 30px;
}
</style>