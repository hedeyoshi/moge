<template>
  <div class="moge">
    <Header logo="MogeMoge"/>
    <h1>This is an Moge page</h1>
    <HelloWorld msg="もげもげもげもげ"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'moge',
  components: {
    Header,
    HelloWorld
  }
}
</script>
