<template>
  <ul class="list-word">
    <li class="word">
      <h4>name1</h4>
      <p>fgbndfgbdfgb</p>
      <cite>article</cite>
    </li>
    <li class="word">
      <h4>name2</h4>
      <p>fgbndfgbdfgb</p>
      <cite>article</cite>
    </li>
    <li class="word">
      <h4>name3</h4>
      <p>fgbndfgbdfgb</p>
      <cite>article</cite>
    </li>


  </ul>
</template>

<script>
export default {
  name: "list-word",
  components: {}
}
</script>

<style>
.list-word {
  padding: 15px 50px;
}

.word {
  list-style: none;
  margin: 20px 10px;
  font-size: 18px;
}
</style>