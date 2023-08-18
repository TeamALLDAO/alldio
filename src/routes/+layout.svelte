<script>
	import Footer from '../components/Footer.svelte';
import Header from './Header.svelte';
	import './styles.css';
</script>

<div class="app">
	<Header />

	<main class="w-screen md:w-[70%] m-auto pt-[100px]">
		<slot />
	</main>

	<Footer/>
</div>

