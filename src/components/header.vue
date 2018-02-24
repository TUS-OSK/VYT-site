<template>
	<div class="container">
		<div class="title">{{ title }}</div>
		<div v-on:click="hoge"></div>
	</div>
</template>

<script>
	module.exports = {
		props: ["title"],
		components: {
		},
		data: function() {
			return {
			}
		},
		methods: {
			hoge: function() {
				console.log(this)
			}
		},
		computed: {
		}
	}
</script>

<style scoped>
	.container {
		border-bottom: 2px solid #603CC0;
		color: #ccc;
		height: 100px;
	}
	.title {
		color: #a73F77;
		/*color: #971F57;*/
		color: #603CC0;
		font-size: 30px;
		text-shadow: 
			#150E4C calc(1px) 0px,  #150E4C calc(-1px) 0px,
			#150E4C 0px calc(-1px), #150E4C 0px calc(1px),
			#150E4C calc(1px) calc(1px) , #150E4C calc(-1px) calc(1px),
			#150E4C calc(1px) calc(-1px), #150E4C calc(-1px) calc(-1px),
			#150E4C 1px calc(1px),  #150E4C -1px calc(1px),
			#150E4C 1px calc(-1px), #150E4C -1px calc(-1px),
			#150E4C calc(1px) 1px,  #150E4C calc(-1px) 1px,
			#150E4C calc(1px) -1px, #150E4C calc(-1px) -1px;
	}
</style>
