<template>
  <header class="Navigation">
    <!-- <h1>{{ logo }}</h1> -->
    <nav>
      <ul>
        <li><router-link to="/" exact>Home</router-link></li>
        <li><router-link to="/About" exact>About</router-link></li>
        <li><router-link to="/Works" exact>Works</router-link></li>
        <li><router-link to="/Contact" exact>Contact</router-link></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: 'Navigation',
  props: {
    logo: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>

.Navigation {
  position: sticky;
  bottom: 0;
  left: 0;
  right: 0;
  height: 48px;
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
}


</style>