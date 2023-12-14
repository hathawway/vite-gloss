<template>
  <ul id="list-word">
    <li class="word">
      <h4>name1</h4>
      <p>fgbndfgbdfgb</p>
      <cite>article</cite>
    </li>
    <li class="word">
      <h4>name2</h4>
      <p>fgbndfgbdfgb</p>
      <cite>article</cite>
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
#list-word {

}

.word {
  list-style: none;
  //border: 3px solid darkslategray;
  outline: none;
  padding: 10px 20px;
  margin: 10px;
}
</style>
