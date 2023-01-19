<script setup lang="ts">
import FlexItem from "@/components/flex-item.vue";
</script>

<template>
	<main class="flex">
		<div class="content">
			<FlexItem />
		</div>
	</main>
</template>

<style>
.flex {
	display: flex;
	width: 100vw;
	height: 100vh;
	justify-content: center;
	align-items: center;
}

.content > div {
	background-color: #1a1725;
	opacity: 0.9;
}

.content {
	display: flex;

	flex-direction: row;
	align-items: stretch;

	width: 47vw;
	height: 80vh;
	gap: 3px;
	padding: 8px;
	background-image: url("images/content.png");
	background-size: 100% 100%;
	background-repeat: no-repeat;
}

@media (max-width: 700px) {
	.content {
		height: 45vh;
		width: 55vw;
	}
}
</style>
