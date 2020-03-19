<template>
	<div id="app">
		<UnComposantQuiAffiche :valueToShow="textDataquelqueChose" />
		<InputText @changeText="changeMyText" />
	</div>
</template>

<script>
	import InputText from "./components/InputText";
	import UnComposantQuiAffiche from "./components/UnComposantQuiAffiche";

	export default {
		name: "App",
		components: {
			InputText,
			UnComposantQuiAffiche
		},
		data() {
			return {
				textDataquelqueChose: "wesh je suis là, mais écrit !"
			};
		},
		methods: {
			changeMyText(valRecuDuInput) {
				this.textDataquelqueChose = valRecuDuInput;
			}
		}
	};
</script>

<style>
	#app {
		font-family: Avenir, Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		text-align: center;
		color: #2c3e50;
		margin-top: 60px;
	}
</style>
