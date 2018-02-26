<template>
	<div class="root-container">
		<Top />
		<!-- <Page /> -->
		<!-- <Grimoire /> -->
	</div>
</template>

<script>
	const store = require("../store.js")

	const Top = require("./top.vue")
	const Page = require("./page-template.vue")
	const Grimoire = require("./grimoire.vue")

	module.exports = {
		store,
		components: {
			Top,
			Page,
			Grimoire
		},
		data: function() {
			return {
			}
		},
		computed: {
		}
	}
</script>

<style scoped>
	.root-container {
		background-color: #f9efd5;
		/*background: linear-gradient(to right bottom, #603CC0, #f9efd5);*/
		color: #978b69;
		color: #746641;
		/*font-family: 'Patrick Hand', cursive;*/	/* 見辛え */
		/*font-family: 'Itim', cursive;*/
		/*font-family: 'Comfortaa', cursive;*/
	}
</style>
