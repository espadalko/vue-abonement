<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <Test1 size="12" level="3" step="30"/>
    <Test1 />
    <Test1 class="indicator" grid="true" size="16" level="12" step="30"/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Test1 from './components/Test1.vue'

export default {
  name: 'app',
  components: {
    // HelloWorld,
    Test1
  }
}
</script>

<style lang="stylus">
#app
  font-family 'Avenir', Helvetica, Arial, sans-serif
  -webkit-font-smoothing antialiased
  -moz-osx-font-smoothing grayscale
  color #2c3e50
.indicator
  height 30px
</style>
