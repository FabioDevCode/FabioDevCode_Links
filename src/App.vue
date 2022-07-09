<template>
	<Header />
	<Link />
	<Projet />




</template>
<!----------Template / Script---------->
<script>
	import Header from './components/Header.vue';
	import Link from './components/Link.vue';
	import Projet from './components/Projet.vue';


	export default {
    name: "FabioDevCode",
    components: { Header, Link, Projet },
		data() {
			return {

			}
		}
	}
</script>
<!----------Script / Style---------->
<style>
	@import './assets/reset.css';

</style>
