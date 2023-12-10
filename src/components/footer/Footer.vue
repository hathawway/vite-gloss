<template>
  <div class="footer-info">
    <p class="copyright">&copy; 2023 Alex Bukov</p>
  </div>
</template>

<script>
export default {
  name: "FooterComponent",
  components: {}
}
</script>

<style>
.footer-info {
  flex: 0 0 auto;
  background-color: #343434;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

.copyright {
  font-size: 20px;
  padding: 15px;
  font-weight: 900;
  color: white;
}


</style>
