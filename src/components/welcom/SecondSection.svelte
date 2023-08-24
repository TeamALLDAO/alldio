<script>
	const info = [
		'Connect your superhero wallet',
		'Add members to your dao',
		'Click on create dao and follow the prompts',
		'create proposals, manage funds, enjoy the dao'
	];
</script>

<div class="">
	<h2 class="font-bold text-xl">How To Get Started</h2>
	<p class="w-1/3 mb-4">
		Creating and managing a DAO is easy with our platform. You can create a DAO in just a few clicks
	</p>

	<div class=" columns-2">
		{#each info as inf, index}
			<div class=" flex gap-2 mb-4 items-center bg-white p-4">
				<h1 class="font-bold">{index + 1}</h1>
				<p>{inf}</p>
			</div>
		{/each}
	</div>

	<div class="flex justify-center my-4">
		<button
			class="w-[340px] bg-[#FF4D4D] h-[50px] py-1 text-white rounded-lg capitalize font-semibold text-xl"
		>
			create a dao</button
		>
	</div>
</div>
