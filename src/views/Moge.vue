<template>
  <div class="moge">
    <Header logo="MogeMoge"/>
    <h1>This is an Moge page</h1>
    <HelloWorld msg="もげもげもげもげ"/>
    <Footer logo="moge footer" />
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import HelloWorld from '@/components/HelloWorld.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'moge',
  components: {
    Header,
    HelloWorld,
    Footer
  }
}
</script>
