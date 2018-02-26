<template>
	<div class="page-container">
		<Header title="Top" />
		<div class="page-content">
			<!-- <Grimoire /> -->
		</div>
		<Footer />
	</div>
</template>

<script>
	const Header = require("./header.vue")
	const Footer = require("./footer.vue")
	const Grimoire = require("./grimoire.vue")

	module.exports = {
		props: [],
		components: {
			Header,
			Footer,
			Grimoire
		},
		data: function() {
			return {
			}
		},
		methods: {
		},
		computed: {
		}
	}
</script>

<style scoped>
	.page-container {
		min-height: 100vh;
		display: flex;
		flex-direction: column;
	}
	.page-content {
		flex-grow: 1;
		/*padding: 20px;*/
		background: linear-gradient(#603CC0, #f9efd5);
		/*background: linear-gradient(to right bottom, #603CC0, #f9efd5);*/
	}
</style>
