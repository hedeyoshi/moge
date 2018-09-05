<template>
  <header class="Header">
    <h1>{{ logo }}</h1>
    <nav>
      <ul>
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/about">About</router-link></li>
        <li><router-link to="/moge">Moge</router-link></li>
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
.Header {
  position: -webkit-sticky;
  position: sticky;
  top: 0;
  width: 100vw;
  background-color: #33ff00;
}
</style>