<template>
  <div id="app">
    
<!--
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/moge">Moge</router-link>
    </div>
 -->
<!-- ヘッダをAppにもってきて楽しようとしたあたりで集中力が切れました。
来週のおれがんばってね。 -->

    <section class="contents">
      <!-- ↓ここにrouter.jsで指定したページが描画される -->
      <router-view/>
    </section>  

    <Header logo="Logo"/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue';

export default {
  components: {
    Header,
  },
};
</script>

<style>
@import url(//yui.yahooapis.com/3.18.1/build/cssreset/cssreset-min.css);
* {
  box-sizing: border-box;
}
#app {
  width: 100vw;
  height: 100vh;
  display: grid;
  grid-template-rows: 1fr 48px;

  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #ccc;
}
.contents {
  max-height: calc(100vh - 48px);
  overflow-x: scroll;
}
.contents > div {
  min-height: calc(100vh - 48px);
  padding: 1rem;
}
.header {
}

.itemList {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  grid-auto-columns: minmax(150px, auto);
  grid-template-rows: 1fr;
  grid-auto-rows: 1fr;
  column-gap: 5px;
  row-gap: 5px;
  background-color: $light-gray;
  padding: 5px;
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
