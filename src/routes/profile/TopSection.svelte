<script>
	import AddMeber from '../../components/popups/AddMeber.svelte';
	import Exchange from '../../components/popups/Exchange.svelte';
</script>

<section class="flex flex-col md:flex-row md:items-center justify-between md:gap-3">
	<div class=" md:w-[70%]">
		<h2 class="text-xl font-bold mb-2">Decentralized Social Media Dao</h2>
		<p>
			Decentralized Social Media DAO is a DAO focused on creating a decentralized social media
			platform that prioritizes user privacy and content ownership. Members can vote on development
			proposals and features to add to the platform.
		</p>
	</div>
	<div class="flex gap-2 items-center md:ml-3 mt-3 md:mt-0">
		<AddMeber />
		<Exchange />
	</div>
</section>
