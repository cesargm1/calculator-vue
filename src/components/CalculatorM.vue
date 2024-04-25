<template>
	<div class="container">
		<section class="result">
			<input readonly v-model="current" type="number" />
		</section>

		<section class="buttons-calculator">
			<button class="button">1</button>
			<button class="button">2</button>
			<button class="button">3</button>
			<button class="button">x</button>

			<button class="button">4</button>
			<button class="button">5</button>
			<button class="button">6</button>
			<button class="button">/</button>

			<button class="button">7</button>
			<button class="button">8</button>
			<button class="button">9</button>
			<button class="button">-</button>

			<button class="button">0</button>
			<button class="button">=</button>
			<button class="button">C</button>
			<button class="button">+</button>
		</section>
	</div>
</template>

<script setup>
import { ref } from "vue";
const current = ref(0);
</script>

<style scoped>
.container {
	max-width: 700px;
	display: grid;
	gap: 0.5em;
	background-color: rgb(183, 175, 175);
	box-shadow: 2px 2px 10px rgb(50, 50, 50), 2px 2px 10px inset rgb(86, 83, 83);
	padding: 1em;
}

.result {
	width: 100%;
	background-color: white;
	padding: 1em;
}

input {
	width: 100%;
	border: none;
	text-align: center;
	font-size: 1.5em;
}

input:focus {
	outline: none;
}

.buttons-calculator {
	display: grid;
	grid-template-columns: repeat(4, 1fr);
	gap: 0.5em;
}

button {
	cursor: pointer;
	padding: 2em;
	background-color: rgb(36, 34, 34);
	color: rgb(230, 226, 226);
	font-size: 2em;
	box-shadow: 2px 2px 10px rgb(50, 50, 50), 2px 2px 10px inset rgb(86, 83, 83);
	backdrop-filter: blur(7.1px);
}

button:hover {
	border: 1px solid rgba(255, 255, 255, 0.3);
}
</style>
