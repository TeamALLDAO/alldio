<script>
	let showForm = false;
</script>

<button
	class="py-2 px-5 rounded-lg border-2 h-[40px] whitespace-nowrap"
	on:click={() => (showForm = !showForm)}>Add Member</button
>

{#if showForm}
	<div
		class="fixed md:right-5 top-16 rounded-lg right-0 bg-gray-200 p-5 w-full md:w-[30%] z-40 overflow-y-scroll hide-scroll"
	>
		<div class="flex justify-between items-start">
			<div>
				<h2 class=" font-bold mb-2">Add Member</h2>
				<p>Enter information of the user you would like to add</p>
			</div>
			<button on:click={() => (showForm = !showForm)}>x</button>
		</div>

		<div>
			<input class=" w-full p-2 my-2 rounded-full" placeholder="Target Address" />
			<input class=" w-full p-2 my-2 rounded-full" placeholder="Amount" />
			<button class=" w-full p-2 my-2 rounded-full bg-[#181818] text-white">submit</button>
		</div>
	</div>
	<button
		on:click={() => (showForm = !showForm)}
		class="w-screen h-screen bg-[#00000077] fixed left-0 top-0"
	/>
{/if}
