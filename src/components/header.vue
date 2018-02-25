<template>
	<div class="header-container">
		<!-- <div v-on:click="hoge"></div> -->
		<!-- <div><div id="logo"></div></div> -->
		<div class="buttons">
		<!-- <div class="title">{{ title }}</div> -->
			<Button text="Home" :click="hoge" />
			<Button text="News" :click="hoge" />
			<Button text="YouTube" :click="hoge" />
			<Button text="Contact" :click="hoge" />
			<Button text="Downloads" :click="hoge" />
		</div>
	</div>
</template>

<script>
	const Button = require("./header-button.vue")

	module.exports = {
		props: ["title"],
		components: {
			Button
		},
		data: function() {
			return {
			}
		},
		methods: {
			hoge: function(event) {
				console.log("びゃぁぁあああ")
			}
		},
		computed: {
		}
	}
</script>

<style scoped>
	.header-container {
		border-bottom: 2px solid #603CC0;
		color: #ccc;
		/*height: 100px;*/
		display: flex;
	}
	.header-container * {
		width: 100%;
	}
	#logo {
		/*background-image: url(../../../grimoire-logo.svg);*/
		/*background-image: url(https://grimoire.gl/css/images/logo-icon.svg);*/
		width: 50px;
		height: 100%;
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
		text-align: center;
	}
	.buttons {
		display: flex;
		justify-content: space-around;
		align-items: flex-end;
		/*border-top: 2px solid #603CC0;*/
	}
	.buttons * {
		border-left: 2px solid #603CC0;
	}
	.buttons :last-child {
		border-right: 2px solid #603CC0;
	}
</style>
