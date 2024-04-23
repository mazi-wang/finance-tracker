<template>
	<section class="flex items-center justify-between mb-10">
		<h1 class="text-4xl font-extrabold">Summary</h1>
		Index page!

		<div>
			<USelectMenu v-model="selectedView" :options="transactionViewOption" />
		</div>
	</section>

	<section
		class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 sm:gap-16 mb-10">
		<Trend />
		<Trend />
		<Trend />
		<Trend />
	</section>
</template>

<script lang="ts" setup>
	import { transactionViewOption } from '~/constants'
	const selectedView = ref(transactionViewOption[1])
</script>

<style scoped></style>
