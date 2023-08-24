<script>
	import LineChart from '../../components/charts/LineChart.svelte';
import ArrowDown from '../../components/icons/ArrowDown.svelte';
	import TopSection from './TopSection.svelte';

	let firstView = true;
</script>

<div class="p-5">
	<TopSection />

	<div class="border-b-2 border-gray-300 flex gap-2 my-6">
		<button
			on:click={() => (firstView = true)}
			class={` font-bold border-b ${
				firstView ? 'text-gray-900 border-gray-900' : 'text-gray-300'
			} px-5 py-2`}>Details</button
		>
		<button
			on:click={() => (firstView = false)}
			class={`font-bold border-b ${
				!firstView ? 'text-gray-800 border-gray-900' : 'text-gray-300'
			} px-5 py-2`}>Proposals</button
		>
	</div>

	<section>
		<div class="md:w-[30%] mt-10">
			<div class="flex justify-between">
				<div>Date created :</div>
				<div>12/03/2022</div>
			</div>
			<div class="flex justify-between">
				<div>Community :</div>
				<div>www.discord.com</div>
			</div>
			<div class="flex justify-between">
				<div>Proposals :</div>
				<div>4k+</div>
			</div>
			<div class="flex justify-between">
				<div>Token price :</div>
				<div>$1</div>
			</div>
		</div>

		<div class="my-4 mt-10">
			<div class="flex items-center gap-2">
				<h2 class="font-bold text-xl">Member</h2>
				<div
					class="grid place-content-center bg-gray-200 rounded-full p-2 ml-3 text-xs w-[30px] h-[30px]"
				>
					4
				</div>
			</div>

			<div class="flex justify-between my-2 items-center bg-gray-100 p-3 rounded-lg mt-4">
				<div class="flex gap-2 items-center">
					<img src="/Frame 14.png" alt="" class="w-[50px] h-[50px] rounded-full" />
					<p>10SBVUubd...Xdxsiw928</p>
				</div>

				<div class="rounded-full py-2 px-4 bg-gray-200 font-bold">Members</div>
			</div>
			<div class="flex justify-between my-2 items-center bg-gray-100 p-3 rounded-lg">
				<div class="flex gap-2 items-center">
					<img src="/Frame 14.png" alt="" class="w-[50px] h-[50px] rounded-full" />
					<p>10SBVUubd...Xdxsiw928</p>
				</div>

				<div class="rounded-full py-2 px-4 bg-gray-200 font-bold">Members</div>
			</div>
			<div class="flex justify-between my-2 items-center bg-gray-100 p-3 rounded-lg">
				<div class="flex gap-2 items-center">
					<img src="/Frame 14.png" alt="" class="w-[50px] h-[50px] rounded-full" />
					<p>10SBVUubd...Xdxsiw928</p>
				</div>

				<div class="rounded-full py-2 px-4 bg-gray-200 font-bold">Members</div>
			</div>
		</div>
	</section>

	<section class=" mt-10">
		<h2 class="my-4 font-bold text-xl">Treasury</h2>

		<div>
			<p>Total Value Locked : $1,203,478.25</p>
			<p>Contract address : oxf26b...ca523</p>
		</div>
	</section>

	<section class="my-4 mt-10 rounded-full">
		<select class=" w-[200px] bg-gray-100 p-3 rounded-full pr-3">
			<option class="flex justify-between">Proposals</option>
		</select>

        <div>
            <LineChart/>
        </div>
	</section>
</div>
