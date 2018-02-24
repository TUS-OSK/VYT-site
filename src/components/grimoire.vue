<template>
	<div class="container">
		aaa
		<script type="text/goml">
			<goml width="300" height="300">
				<scene>
					<camera class="camera" position="0,0,5">
						<camera.components>
							<MouseCameraControl/>
						</camera.components>
					</camera>
					<light intensity="3" />
					<!-- <model src="http://ci.grimoire.gl/tf/Duck/glTF/Duck.gltf" /> -->
					<!-- <model src="http://localhost:3000/grimoire-chan.gltf" /> -->
					<model src="http://localhost:3000/grimoire-chan.gltf" />
					<!-- <mesh geometry="cube" position="0,0,0" color="#00f" sun="n(0,0,-1)" ></mesh> -->
				</scene>
			</goml>
		</script>
		bbb
	</div>
</template>

<script>
	// require("grimoirejs-preset-basic")
	module.exports = {
		props: [],
		components: {
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
	.container {
	}
</style>
