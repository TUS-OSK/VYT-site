<template>
	<div class="root-container">
		<!-- <Top /> -->
		<!-- <Page /> -->
		<GL />
	</div>
</template>

<script>
	const store = require("../store.js")

	const Top = require("./top.vue")
	const Page = require("./page-template.vue")
	const GL = require("./grimoire.vue")

	module.exports = {
		store,
		components: {
			Top,
			Page,
			GL
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
		color: #978b69;
		color: #746641;
	}
</style>
