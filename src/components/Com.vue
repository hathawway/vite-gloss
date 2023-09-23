<template>
  <div id="Com">
    <h1>hello</h1>
    <div>
      <button @click="addLike">Like add</button>
      <button @click="addDislike">Dislike add</button>
    </div>
    <div>likes - {{ likes }}</div>
    <div>dislikes - {{ dislikes }}</div>
  </div>
</template>

<script>
export default {
  name: "Com",
  data() {
    return {
      likes: 0,
      dislikes: 0,
    }
  },
  methods: {
    addLike() {
      this.likes += 1
    },
    addDislike() {
      this.dislikes += 1
    }
  },
}
</script>