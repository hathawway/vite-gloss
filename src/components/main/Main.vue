<template>
  <div class="main-words">
    <ListWord v-if="!store.getters.getGraphEnabled"/>
    <GraphView v-else/>
  </div>
</template>

<script>
import ListWord from "./ListWord.vue";
import GraphView from "./GraphView.vue";
import { store } from "../../store/main_page.js";

export default {
  name: "MainComponent",
  data() {},
  components: {
    GraphView: GraphView,
    ListWord: ListWord,
  },
  computed: {
    store() {
      return store
    },
  },
}
</script>

<style>
.main-words {
  flex: 1 0 auto;
  background-color: #343434;
}
</style>
