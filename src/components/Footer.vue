<template>
  <footer class="Footer">
    <address>{{ logo }}</address>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  props: {
    logo: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.Footer {
  background-color: #333333;
  color: #ffffff;
  text-align: center;
  padding: 2rem;
}
</style>
