<script setup lang="ts">
import FlexItem from "@/components/flex-item.vue";
</script>

<template>
	<div class="title">
		<h1>FLEXBOX TESTER</h1>
	</div>
	<div class="display">
		<div class="contentInput">
			<p>Selecione o componente que deseja fazer as alterações.</p>
			<div class="selectButton">
				<select>
					<option value="">-- Escolha uma opção --</option>
					<option value="dog">Content</option>
					<option value="cat">Items</option>
				</select>
			</div>
			<p>
				Incremente no input a propriedade e a atribuição desejada. OBS: Caso queira alterar alguma propriedade
				já presente no código. basta digita-lá novamente com a nova atribuição.
			</p>
			<input
				type="text"
				placeholder="Coloque seu código aqui!"
			/>
			<div class="cod">Nessa div será exibido as linhas de cód já feitas.</div>
		</div>
		<main class="flex">
			<div class="content">
				<FlexItem />
			</div>
		</main>
	</div>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Barlow&display=swap");
.title {
	display: flex;
	width: 100vw;
	height: 10vh;
	justify-content: center;
	margin-bottom: 18px;
}
.display {
	display: flex;
	width: 100vw;
	height: 90vh;
	gap: 56px;
	justify-content: center;
	align-items: center;
	flex-wrap: wrap;
}
.flex {
	display: flex;
	align-items: center;
}
.contentInput {
	display: flex;
	flex-direction: column;
	align-items: center;
	background-color: #110e18;
	width: 480px;
	height: 75vh;
	border-radius: 30px;
	gap: 9px;
	font-family: "Barlow";
	font-style: normal;
	font-weight: 400;
	font-size: 16px;
	line-height: 19px;
	text-align: center;
	letter-spacing: -0.03em;
	color: #decffb;
}
p {
	max-width: 350px;
	font-family: "Barlow";
	font-style: normal;
	font-weight: 400;
	font-size: 16px;
	line-height: 19px;
	text-align: center;
	letter-spacing: -0.03em;
	color: #decffb;
}
input {
	width: 332px;
	height: 38px;
	border-radius: 14px;
	background-color: #1a1725;
	border: #decffb 2px solid;
	font-family: "Barlow";
	color: #decffb;
	padding: 0 5px;
}
.selectButton select {
	width: 332px;
	height: 38px;
	border-radius: 14px;
	background-color: #1a1725;
	border: #decffb 2px solid;
	font-family: "Barlow";
	color: #decffb;
	padding: 0 5px;
}
.content > div {
	background-color: #1a1725;
	opacity: 0.9;
}
.content {
	display: flex;
	flex-direction: row;
	align-items: stretch;
	width: 40vw;
	height: 70vh;
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
