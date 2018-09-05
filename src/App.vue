<template>
  <div id="app">
    
    <Header logo="Logo"/>
<!--
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/moge">Moge</router-link>
    </div>
 -->

    <!-- ↓ここにrouter.jsで指定したページが描画される -->
    <router-view/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'

export default {
  components: {
    Header
  }
}

</script>

<style>
@import url(//yui.yahooapis.com/3.18.1/build/cssreset/cssreset-min.css);
* {
  box-sizing: border-box;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #ccc;
}
.home {
  background-color: #eeddcc;
}
.about {
  background-color: #ccffdd;
}
.moge {
  background-color: #998877;
}
</style>
