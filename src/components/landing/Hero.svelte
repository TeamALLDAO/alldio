<script>
	import { onMount } from "svelte";


	import { fly } from "svelte/transition";


    let animate = false
    onMount(()=>{
        animate =true
    });

</script>



<section class="p-5 flex flex-col md:flex-row min-h-screen">
<div>
    <h2 class="text-2xl font-bold mb-5">Level Up Your Community With <span class="custom-text">AllDAO</span> - The Ultimate DAO Platform!</h2>
    <p class="mb-5" >Elevate your community's potential with AllDAO. Empowering leaders like you with a sophisticated platform that streamlines decision-making, funds management, and fosters collaboration.</p>
    <button class="border-2 border-blue-800 custom-text py-2 px-5 rounded-lg">Create Dao</button>
</div>

{#if animate}
<div transition:fly={{ y: -200, duration: 100, delay: 100 }}>
    <img src="/top.png" alt="" class=" object-cover"/>
</div>
{/if}
</section>