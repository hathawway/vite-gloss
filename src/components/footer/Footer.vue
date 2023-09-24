<template>
  <div id="footer">
    <hr class="hr-shadow">
    <h5>&copy; 2023 hathawway</h5>
  </div>
</template>

<script>
export default {
  name: "footer",
  components: {}
}
</script>

<style>
#footer {
  background-color: rgba(216, 241, 211, 0.99);
  padding: 10px 30px;
  font-size: 18px;

  position: absolute;
  bottom: 0;
  width: 100%;
}

.hr-shadow {
  margin: 10px 0;
  padding: 0;
  height: 10px;
  border: none;
  border-top: 1px solid #333;
  box-shadow: 0 10px 10px -10px #8c8b8b inset;
}

h5 {
  display: flex;
  align-items: center;
  justify-content: center;
}

</style>