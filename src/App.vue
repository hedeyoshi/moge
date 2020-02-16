<template>
  <div id="app">

    <section class="contents">
      <router-view/>
    </section>  

    <Navigation logo="Logo"/>
  </div>
</template>

<script>
import Navigation from '@/components/Navigation.vue';

export default {
  components: {
    Navigation,
  },
};
</script>

<style>
@import url(//yui.yahooapis.com/3.18.1/build/cssreset/cssreset-min.css);
* {
  box-sizing: border-box;
}
#app {
  /* width: 100vw;
  height: 100vh; */
  /* display: grid;
  grid-template-rows: 1fr 48px; */

  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #ccc;
}
.contents {
  min-height: 100vh
  /* max-height: calc(100vh - 48px);
  overflow-x: scroll; */
}
.contents > div {
  min-height: 100vh
  /* min-height: calc(100vh - 48px);
  padding: 1rem; */
}

/* あとで削除する */
.home {
  background-color: #eeddcc;
}
.about {
  background-color: #ccffdd;
}
.works {
  background-color: #725c46;
}
.contact {
  background-color: #9ad877;
}
</style>
