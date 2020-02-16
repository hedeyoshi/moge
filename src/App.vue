<template>
  <div id="app">
    <section class="contents">
      <div class="grad">
        <router-view />
      </div>
    </section>
    <Navigation />
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

<style lang="scss">
@import url(//yui.yahooapis.com/3.18.1/build/cssreset/cssreset-min.css);
@import url('//fonts.googleapis.com/css?family=M+PLUS+1p&display=swap');
@import url('https://fonts.googleapis.com/css?family=Roboto&display=swap');
/* reset */
* {
  box-sizing: border-box;
}
#app {
  font-family: 'M PLUS 1p', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #ccc;
}
.contents {
  background-image: url(./assets/bg.jpg);
  background-position: center center;
  background-size: 200%;
  min-height: 100vh;
  font-size: 16px;
  color: #fff;
  text-shadow: 0px 1px 4px rgba(0, 0, 0, 0.24);
  & > div {
    max-height: 100vh;
    overflow: auto;
    padding: 5rem 1rem 5rem;
  }
}
.grad {
  width: 100vw;
  height: 100vh;
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(
    36.5deg,
    rgba(93, 190, 255, 0.8),
    rgba(161, 89, 255, 0.8),
    rgba(255, 75, 195, 0.8)
  );
  background-size: 600% 600%;
  animation: gradAnimation 16s ease infinite;
}
.title {
  margin-bottom: 1.6rem;
  font-family: 'Roboto', sans-serif;
  font-size: 4rem;
  font-weight: bold;
  line-height: 1;
  word-break: break-all;
  overflow-wrap: break-word;
}
.icon {
  width: 94px;
  height: 94px;
  border: 4px solid #fff;
  border-radius: 64px;
  box-shadow: 0px 1px 4px rgba(0, 0, 0, 0.24);
}
@keyframes gradAnimation {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
</style>
