<template>
	<Header />

	<Link />

	<Projet />

	<Footer />
</template>
<!----------Template / Script---------->
<script>
	import Header from './components/Header.vue';
	import Link from './components/Link.vue';
	import Projet from './components/Projet.vue';
	import Footer from './components/Footer.vue';

	export default {
    name: "FabioDevCode",
    components: { Header, Link, Projet, Footer },
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
