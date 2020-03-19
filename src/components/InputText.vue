<template>
	<div>
		<input type="text" value="" @input="ecrisQuelqueChose" />
	</div>
</template>

<script>
	export default {
		props: {
			defaultValue: {
				type: String,
				default: ""
			}
		},
		methods: {
			ecrisQuelqueChose(e) {
				console.log(e.target.value);
				this.$emit("changeText", e.target.value);
			}
		}
	};
</script>

<style lang="scss" scoped></style>
