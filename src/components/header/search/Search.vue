<template>
  <div class="search search-btn">
    <button class="btn-btn">Глоссарий</button>
    <button class="btn-btn">Граф</button>
  </div>
  <div class="search search-str">
    <input
        type="search"
        class="input-search"
        placeholder="Поиск"
        v-model="searchText"
    >
    <button
        class="btn-search"
        v-on:click="search">Поиск
    </button>
  </div>
  <div class="search search-name">
    <button class="btn-btn">Alex Bukov</button>
  </div>

</template>

<script>
import {GetPostsViaAPI, SearchPostsViaAPI} from "../../../api/glossary_api.js";
import {store} from "../../../store/main_page.js";

export default {
  name: "search",
  data() {
    return {
      searchText: "",
    }
  },
  components: {},
  methods: {
    search() {
      SearchPostsViaAPI(this.searchText)
    },
    clear() {
      GetPostsViaAPI()
    }
  },
  computed: {
    store() {
      return store
    },
  },
}
</script>

<style>
.search-btn {

}

.btn-btn {
  background-color: white;
  color: rgba(2, 0, 0, 0.99);
  padding: 10px 20px;
  border-radius: 5px;
  border: none;
  margin: 5px;
  font-size: 16px;
}

.btn-btn:hover {
  background-color: #918f8f;
}

.btn-search {
  background-color: #918f8f;
  color: rgba(2, 0, 0, 0.99);
  padding: 10px 20px;
  border-radius: 5px;
  border: none;
  margin: 5px;
  font-size: 16px;
}

.btn-search:hover {
  background-color: white;
}

.search {
  display: flex;
  justify-content: space-around;
}

.search-str {

}

.search-name {

}

.input-search {
  width: 550px;
  padding: 10px 10px;
  border-radius: 5px;
  border: none;
  font-size: 16px;
  color: #020000;
  background-color: #fff;

}

.input-search::placeholder {
  font-size: 18px;
  color: darkslategray;
}

[data-hint] {
  position: relative;
}

[data-hint]::after {
  opacity: 0;
  width: max-content;
  color: #FFFFFF;
  background-color: rgba(0, 0, 0, .7);
  border-radius: 6px;
  padding: 10px;
  content: attr(data-hint);
  font-size: 12px;
  font-weight: 400;
  line-height: 1em;
  position: absolute;
  bottom: -70px;
  left: 50%;
  transform: translate(-50%, -100%);
  pointer-events: none;
  transition: opacity 0.2s;
}

[data-hint]:hover::after {
  opacity: 1;
}

</style>
