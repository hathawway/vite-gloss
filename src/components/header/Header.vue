<template>
  <div id="header">
    <Search/>
    <button class="btn-list">Показать список всех доступных слов</button>
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
#header {
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: rgba(216, 241, 211, 0.99);
  padding: 10px;
}

.btn-list {
  background-color:  rgba(216, 241, 211, 0.99);
  border: none;
  border-bottom: 3px solid darkslategray;
  outline: none;
  font-size: 14px;
  color: darkslategray;
  font-weight: bold;
  letter-spacing: 1px;
}
</style>