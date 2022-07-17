<template>

	<Card />

</template>
<!----------Template / Script---------->
<script>
	import Card from './components/Card.vue';

	export default {
		name: "FabioDevCode",
		components: { Card },
	}
</script>
<!----------Script / Style---------->
<style>
	@import './assets/reset.css';

	#app {
		height: 100vh;
		min-height: max-content;
		width: 100%;
		min-width: 320px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
</style>