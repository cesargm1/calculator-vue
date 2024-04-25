<template>
	<div>
		<CalculatorM />
	</div>
</template>

<script setup>
import CalculatorM from "./components/CalculatorM.vue";
</script>

<style>
:root {
}
* {
	box-sizing: border-box;
	padding: 0;
	margin: 0;
}

body {
	display: grid;
	place-items: center;
	min-height: 100dvh;
	overflow: hidden;
}
</style>
