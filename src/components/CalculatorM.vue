<template>
	<div class="container">
		<section class="result">
			<input type="number" />
		</section>

		<section class="buttons-calculator">
			<button>1</button>
			<button>2</button>
			<button>3</button>
			<button>x</button>

			<button>4</button>
			<button>5</button>
			<button>6</button>
			<button>/</button>

			<button>7</button>
			<button>8</button>
			<button>9</button>
			<button>-</button>

			<button>0</button>
			<button>=</button>
			<button>C</button>
			<button>%</button>
		</section>
	</div>
</template>

<script setup></script>

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
}
</style>
