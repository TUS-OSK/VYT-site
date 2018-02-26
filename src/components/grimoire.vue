<template>
	<div class="container">
		<script type="text/goml">
			<goml width="400" height="400">
				<scene>
					<camera class="camera" position="0,0,6">
						<camera.components>
							<MouseCameraControl/>
						</camera.components>
					</camera>
					<light intensity="10"/>
					<!-- <model src="http://ci.grimoire.gl/tf/Duck/glTF/Duck.gltf" /> -->
					<!-- <model src="http://localhost:3000/grimoire-chan.gltf" /> -->
					<model position="0,-2,0" rotation="0,180,0" src="https://raw.githubusercontent.com/TUS-OSK/VYT-site/grimoire/gltf/grimoire-chan-cx20.gltf" />
					<!-- <mesh geometry="cube" position="0,0,0" color="#00f" sun="n(0,0,-1)" ></mesh> -->
				</scene>
			</goml>
		</script>
	</div>
</template>

<script>
	module.exports = {
		props: ["width", "height"],
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
