<template>
	<div>Trend</div>
</template>

<script lang="ts" setup>
	defineProps({
		title: String,
		amount: Number,
		lastAmount: Number,
		color: String,
		loading: Boolean,
	})
</script>

<style scoped></style>
