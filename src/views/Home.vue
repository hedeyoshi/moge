<template>
  <div class="home">
    <Header logo="mogeeeeeeeeeeee!!!!!!!!!"/>
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Footer logo="home footer" />
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import HelloWorld from '@/components/HelloWorld.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'home',
  components: {
    Header,
    HelloWorld,
    Footer
  }
}
</script>
