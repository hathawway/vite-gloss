<template>
  <ul id="list-word">
    <li v-for="c in store.getters.getPosts" class="word">
      <h3>{{ c.name }}</h3>
      <p>{{ c.content }}</p>
      <div v-if="c.link">
      </div>
      <div v-else>
      </div>
    </li>
  </ul>
</template>

<script>

import { store } from "../../store/main_page.js";

export default {
  name: "list-word",
  computed: {
    store() {
      return store
    },
  },
  components: {}
}
</script>

<style>
#list-word {
  padding: 15px 50px;
}

.word {
  list-style: none;
  margin: 20px 10px;
  font-size: 18px;
  padding: 15px 15px;
  border-radius: 5px;
  border-style: none;
  background-color: white;
}
</style>
