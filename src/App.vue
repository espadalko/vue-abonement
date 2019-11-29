<template>
	<div id="app">
		<!-- <img alt="Vue logo" src="./assets/logo.png"> -->
		<!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
		<div class="slider">
			<Test1 width="30px" class="test1" /> 
		</div>
<!--     <Test1 size="12" level="3" step="35" height="20" />
	 <Test1 height="20" />
	 <Test1 size="16" level="12" step="35" height="20"/>
	-->    
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
*
	box-sizing border-box
body 
	background-color #333
#app
	font-family 'Avenir', Helvetica, Arial, sans-serif
	-webkit-font-smoothing antialiased
	-moz-osx-font-smoothing grayscale
	color #2c3e50

.slider
	width 700px
	background-color red

</style>
