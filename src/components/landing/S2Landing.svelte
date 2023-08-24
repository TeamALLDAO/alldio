<script>
	import CreateDao from '../popups/CreateDAO.svelte';

	let info_left = `text-end p-3 backdrop-blur-[10px] border-2 m-2 rounded-lg shadow-lg hover:translate-x-[0px] hover:bg-white min-h-[250px] md:h-fit`;
	let info_right = `p-3 backdrop-blur-[10px] border-2 m-2 rounded-lg shadow-lg hover:translate-x-[0px] hover:bg-white  min-h-[250px] md:h-fit`;
	let parent_div = 'relative  flex flex-col gap-5 md:justify-around ';
</script>

<h2 class="text-xl font-bold text-center mb-10">Key Benefits</h2>
<section class="flex justify-between items-center">
	<div class={`${parent_div}`}>
		<div class={`${info_left} md:translate-x-[-50px]`}>
			<div class="flex gap-2 w-full flex-row-reverse">
				<img src="/shild.svg" alt="" class="w-5" />
				<h2>100% Secured</h2>
			</div>
			<p>
				Our cutting-edge security measures guarantee the utmost safety of your community's assets
				and data.
			</p>
		</div>
		<div class={`${info_left} md:translate-x-[-100px]`}>
			<div class="flex gap-2 flex-row-reverse">
				<img src="/finger.svg" alt="" class="w-5" />
				<h2>Easy to use</h2>
			</div>
			<p>
				AllDAO's user-friendly interface makes community management intuitive, enabling everyone to
				participate with ease..
			</p>
		</div>
		<div class={`${info_left} md:translate-x-[-50px]`}>
			<div class="flex gap-2 flex-row-reverse">
				<img src="/wave.svg" alt="" class="w-5" />
				<h2>Flexible</h2>
			</div>
			<p>
				AllDAO adapts to your community's unique needs, providing versatile tools to suit any
				situation or event.
			</p>
		</div>
	</div>
	<div class="absolute -z-10 w-full md:w-1/2 left-0 right-0 m-auto">
		<img src="/midle.png" alt="" class="object-contain" />
	</div>
	<div class={`${parent_div}`}>
		<div class={`${info_right} md:translate-x-[50px]`}>
			<div class="flex gap-2">
				<h2>100% Decentralized</h2>
				<img src="/btc.svg" alt="" class="w-5" />
			</div>
			<p>
				AllDAO embraces full decentralization, ensuring every member's voice and vote matter in
				shaping the community's future..
			</p>
		</div>
		<div class={`${info_right} md:translate-x-[100px]`}>
			<div class="flex gap-2">
				<h2>Cheap</h2>
				<img src="/cheap.svg" alt="" class="w-5" />
			</div>
			<p>
				By leveraging blockchain technology, AllDAO offers cost-effective solutions, saving your
				community from unnecessary expenses.
			</p>
		</div>
		<div class={`${info_right} md:translate-x-[50px]`}>
			<div class="flex gap-2">
				<h2>Fast</h2>
				<img src="/flash.svg" alt="" class="w-5" />
			</div>
			<p>
				Experience seamless transactions and lightning-fast fund transfers with AllDAO's optimized
				platform.
			</p>
		</div>
	</div>
</section>

<div class="flex w-full justify-center my-10">
	<CreateDao />
</div>
