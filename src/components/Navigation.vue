<template>
  <header class="Navigation">
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
    logo: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.Navigation {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  box-shadow: 0 0 32px 0 rgba(0, 0, 0, 0.16);
  font-family: 'Roboto', sans-serif;
  ul {
    display: flex;
    justify-content: center;
    align-items: stretch;
  }
  li {
    flex: 1 0 auto;
  }
  a {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 48px;
    background-color: #fff;
    text-decoration: none;
    transition: ease 0.16s;
    &:link,
    &:visited {
      color: #111111;
    }
    &:active {
    }
    &:hover,
    &:focus {
      color: #ff1940;
    }
  }
  .router-link-active {
    background-color: #deff22;
  }
}
</style>
