<template>
	<div class="page-container">
		<div class="page-content">
			Hello World!
		</div>
	</div>
</template>

<script>
	const Header = require("./header.vue")
	const Footer = require("./footer.vue")

	module.exports = {
		components: {
			Header,
			Footer
		},
		data: function() {
			return {
				msg: "Hello World!"
			}
		},
		computed: {
		}
	}
</script>

<style scoped>
	.page-container {
		background-color: #F00;
		min-height: 100vh;
		display: flex;
		flex-direction: column;
	}
	.page-content {
		flex-grow: 1;
		/*padding: 20px;*/
	}
</style>
