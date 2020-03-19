<template>
	<div>{{ valueToShow }}</div>
</template>

<script>
	export default {
		props: {
			valueToShow: {
				type: String,
				required: true
			}
		}
	};
</script>

<style lang="scss" scoped></style>
