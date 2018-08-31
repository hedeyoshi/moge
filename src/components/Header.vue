<template>
  <header class="Header">
    <h1>{{ logo }}</h1>
    <nav>
      <ul>
        <li><a href="">nav 1</a></li>
        <li><a href="">nav 2</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',
  props: {
    logo: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
