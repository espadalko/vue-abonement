<template>
	<div 
		class="indicator" 
		:style="{width: size * step + 'px', height: height + 'px'}"
	>
		<div 
			class="indicator__level" 
			:style="{
				width: level * step + 'px', 
				height: height + 'px'
			}"
		></div>
		<div 
			class="indicator__grid" 
			:style="{width: step + 'px', height: height + 'px'}"
			v-for="n in emptyArray(size)"
		></div>
	</div>
</template>

<script>
	export default {
		props:{
			size:{type: Number, default: 16},
			level:{type: Number, default: 8},
			step:{type: Number, default: 30},
			height:{type: Number, default: 100}
		},
		data(){
			return {
			}
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

<style lang="stylus">
	color = #70A1CF 
	.indicator
		display flex
		border 1px solid color 
		margin 10px
		&__level
			position fixed
			background-color color
			// margin 2px
			z-index 1
		&__grid
			position relative
			// border 3px solid white
			background-color red
			z-index 2
</style>