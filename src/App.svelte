<script>
	import Header from './components/Header.svelte'
	import Nav from './components/Nav.svelte'
	import Aside from './components/Aside.svelte';
	import Footer from './components/Footer.svelte';
	import Section from './components/Section.svelte';
	import Article from './components/Article.svelte';
	export let name;
</script>

<main>
	<Header/>
	<Nav/>
	<Aside/>
	<Section>
		<Article/>
		<Article/>
	</Section>
	<Footer/>
</main>

<style>
	main {
		text-align: center;
		padding: 0;
		max-width: 240px;
		margin: 0 auto;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>