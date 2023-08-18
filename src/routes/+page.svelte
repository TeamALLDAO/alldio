<script>
	import AboutUs from "../components/landing/AboutUs.svelte";
import Hero from "../components/landing/Hero.svelte";
	import RoadMap from "../components/landing/RoadMap.svelte";
	import S2Landing from "../components/landing/S2Landing.svelte";
	import TogetStarted from "../components/landing/TogetStarted.svelte";

	

</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>

	<Hero/>
	<div class="my-10 w-full h-[20px]"/>
	<S2Landing/>
	<div class="my-10 w-full h-[20px]"/>
	<AboutUs/>
	<div class="my-10 w-full h-[20px]"/>
	<TogetStarted/>
	<div class="my-10 w-full h-[20px]"/>
	<RoadMap/>
	<div class="my-10 w-full h-[20px]"/>



</section>

