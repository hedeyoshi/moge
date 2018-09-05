<template>
  <div class="about">
    <Header logo="aaaaaaaaahhhhhhhhhh!!!!!!!!!"/>
    <h1>This is an about page</h1>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Footer logo="about footer" />
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import HelloWorld from '@/components/HelloWorld.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'about',
  components: {
    Header,
    HelloWorld,
    Footer
  }
}
</script>
