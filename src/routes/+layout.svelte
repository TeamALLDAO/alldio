<script>
	import Footer from '../components/layouts/Footer.svelte';
	import Header from '../components/layouts/Header.svelte';
	import './styles.css';
</script>

<div class="app">
	<Header />

	<main class="w-screen md:w-[70%] m-auto pt-[100px] min-h-screen pb-20">
		<slot />
	</main>

	<Footer />
</div>
