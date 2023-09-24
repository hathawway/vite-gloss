<template>
  <form id="search" action="" method="get">
      <input type="search" class="input" placeholder="Search">
    <button type="submit" class="search-btn">Поиск</button>
  </form>

</template>

<script>
export default {
  name: "search",
  components: {},
  methods: {
  },
}
</script>

<style>
#search {
  display: flex;
  flex-direction: row;
  padding: 20px 50px;
}

.search-btn {
  margin: 0px 5px;
  border: 3px solid darkslategray;
  padding: 15px 30px;
  border-radius: 50px;
  outline: none;
  font-size: 18px;
  color: darkslategray;
  font-weight: bold;
  letter-spacing: 1px;
  background-color:  rgba(216, 241, 211, 0.99);
}

.input {
  width: 400px;
  border: 3px solid darkslategray;
  background: transparent;
  padding: 15px 30px;
  border-radius: 50px;
  outline: none;
  font-size: 18px;
  color: darkslategray;
  font-weight: bold;
  letter-spacing: 1px;
}

::-webkit-input-placeholder { /* Chrome/Opera/Safari */
  color: darkslategray;
  font-family: Roboto;
  letter-spacing: 2px;
  text-transform: uppercase;
}

::-moz-placeholder { /* Firefox 19+ */
  color: darkslategray;
}

:-ms-input-placeholder { /* IE 10+ */
  color: darkslategray;
}

@keyframes animate {
  0% {
    transform: scale(1);
  }
  25% {
    transform: scale(1.2);
  }
  50% {
    transform: scale(1.5);
  }
  75% {
    transform: scale(1.2);
  }
  100% {
    transform: scale(1);
  }
}
</style>