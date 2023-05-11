<template>
  <div class="home">
    <headerBar />
    <!-- <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import headerBar from '@/components/headerBar.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    headerBar
  }
}
</script>
