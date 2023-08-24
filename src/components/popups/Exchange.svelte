<script>
	let showForm = false;
</script>

<button
	on:click={() => (showForm = !showForm)}
	class="bg-[#181818] text-white py-2 px-5 ml-2 h-[40px] rounded-lg">Exchange</button
>
{#if showForm}
	<div
		class="fixed md:right-5 top-16 rounded-lg right-0 bg-gray-200 p-5 w-full md:w-[30%] z-40 overflow-y-scroll hide-scroll"
	>
		<div class="flex justify-between items-start">
			<div>
				<h2 class=" font-bold mb-2">Create proposal</h2>
				<p>Select the type of proposal</p>
			</div>
			<button on:click={() => (showForm = !showForm)}>x</button>
		</div>

		<div>
			<div class="bg-white w-full rounded-lg p-2 my-2">Governor</div>
			<div class="bg-white w-full rounded-lg p-2 my-2">Funding</div>
			<div class="bg-white w-full rounded-lg p-2 my-2">Payment</div>
			<button class=" w-full p-2 my-2 rounded-lg bg-[#181818] text-white">submit</button>
		</div>
	</div>
	<button
		on:click={() => (showForm = !showForm)}
		class="w-screen h-screen bg-[#00000077] fixed left-0 top-0"
	/>
{/if}
