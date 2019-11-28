<template>
	<div class="indicator" :style="{width: size * step + 'px', height: height + 'px'}">
 		<div class="indicator__level" :style="{width: step + 'px', height: height + 'px'}" v-for="n in emptyArray(size)"></div>
	</div>
</template>

<script>
	export default {
		props:{
			size:{type: Number, default: 16},
			level:{type: Number, default: 8},
			step:{type: Number, default: 35},
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
		margin 10px
		&__level
			background-color color
			border 2px solid transparent 
			margin-right 4px
			border-radius 5px
			// margin 2px
</style>