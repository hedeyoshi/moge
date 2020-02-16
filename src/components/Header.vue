<template>
  <header class="Header">
    <!-- <h1>{{ logo }}</h1> -->
    <nav>
      <ul>
        <li><router-link to="/" exact>Home</router-link></li>
        <li><router-link to="/about" exact>About</router-link></li>
        <li><router-link to="/Works" exact>Works</router-link></li>
        <li><router-link to="/Contact" exact>Contact</router-link></li>
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
}
nav {
  height: 48px;
}
ul {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-template-rows: 1fr;
  height: 100%;
}
li {
  display: flex;
  justify-content: center;
  align-items: stretch;
}
a {
  flex: 1 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #fff;
  text-decoration: none;
}
.router-link-active {
  background-color: #cccc22;
}
</style>