<template>
	<div class="indicator" :style="{width: size * step + 'px'}">
		<div class="indicator__level" :style="{width: level * step + 'px'}"></div>
	</div>
</template>

<script>
	export default {
		props:{
			size:{type: Number, default: 16},
			level:{type: Number, default: 8},
			step:{type: Number, default: 30},
		},
	}
</script>

<style lang="stylus">
	color = #70A1CF 
	.indicator
		display flex
		border 1px solid color 
		height 15px
		margin 10px
		&__level
			background-color color
			margin 2px
</style>