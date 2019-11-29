<template>
	<div>
		<div class="slider" :style="{width: width, height: height}">
			<div class="value"></div>
		</div>
 	</div>
</template>

<script>
	export default {
		props:{
			min: 		{type: Number, default: 0},
			max: 		{type: Number, default: 100},
			step: 	{type: Number, default: 1},
			value: 	{type: Number, default: 0},
			width: 	{type: String, default: '300px'},
			height: 	{type: String, default: '30px'}
		},
		methods:{
			emptyArray(num){
				let array =[]
				for (var i = 0; i < num; i++) {
					array.push('')
				}
				return array
			}
		}
	}
</script>

<style lang="stylus" scoped>
	// color = #70A1CF 
	.slider
		// width 100%
		// height 20px
		background-color #fff
</style>