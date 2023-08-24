<script>
	let showForm = false;
	let foundingMembers = [
		{ address: '', percent: '' },
		{ address: '', percent: '' },
		{ address: '', percent: '' }
	];
	function addNewFoundingMembers() {
		return (foundingMembers = [...foundingMembers, { address: '', percent: '' }]);
	}
</script>

<button
	class="border-2 border-blue-800 custom-text py-2 px-5 rounded-lg"
	on:click={() => (showForm = !showForm)}>Create Dao</button
>

{#if showForm}
	<div
		class="fixed md:right-5 top-16 rounded-lg right-0 bg-white p-5 w-full md:w-[40%] z-40 overflow-y-scroll h-[80vh]"
	>
		<h1 class="text-green-800 font-bold my-4">Create DAO form</h1>
		<div class="w-[90%] m-auto">
			<input class=" w-full p-2 border-2 my-2" placeholder="Title" />
			<textarea class=" w-full p-2 border-2 my-2" placeholder="Description" />

			{#each foundingMembers as fm}
				<div class="w-full flex justify-between items-center my-2">
					<input class=" w-[70%] p-2 border-2" placeholder="Founding members address" />
					<input class=" w-[20%] p-2 border-2" placeholder="%" />
				</div>
			{/each}

			<button
				class=" p-2 text-white bg-green-800 text-2xl w-[50px] h-[50px] my-2"
				on:click={addNewFoundingMembers}>+</button
			>

			<input class=" w-full p-2 border-2 my-2" placeholder="Community Link" />

			<label class="flex items-center p-5 bg-[#51ff0032] cursor-pointer hover:bg-blue-600">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					class="w-6 h-6 mr-2"
					viewBox="0 0 20 20"
					fill="currentColor"
				>
					<path d="M10 12a2 2 0 100-4 2 2 0 000 4z" />
					<path
						fill-rule="evenodd"
						d="M10 2a8 8 0 100 16 8 8 0 000-16zm0 14a6 6 0 110-12 6 6 0 010 12z"
						clip-rule="evenodd"
					/>
				</svg>
				<span>Upload Image</span>
				<input type="file" class="hidden" />
			</label>

			<div class="w-full flex justify-end my-2">
				<button class="bg-green-700 text-white py-2 px-5">Submit</button>
			</div>
		</div>
	</div>
	<button
		on:click={() => (showForm = !showForm)}
		class="w-screen h-screen bg-[#00000077] fixed left-0 top-0"
	/>
{/if}
