<script>
	import { fly } from "svelte/transition";

    
let seemore = false;
let team = false;
</script>

<section class="text-center p-3">
    <h2 class="font-bold text-xl">About Us</h2>
    <p class={`my-4 ${!seemore&&"line-clamp-6"}`}>
        At AllDAO, we strive to build a world-class platform for community management and finance, empowering communities to achieve their full potential. We envision creating an ecosystem of thriving DAOs, driving mass adoption of web3 through value-driven community interactions. Our Team comprises of a united community of passionate individuals from diverse backgrounds, brought together by our unyielding commitment to build something significant from our remote corner of the world. As dedicated pioneers, we embrace challenges and opportunities, ready to scale new heights. Our strength lies in our collective determination to bring positive change to community management and finance. Together, we strive to empower every web3 community with the tools and support they need to thrive in the decentralized landscape.
        
    </p>
    <button on:click={()=>seemore=!seemore} class="capitalize">{seemore?'see less': 'see more'}</button>

    <br/>

    <button on:click={()=>team=!team} class="capitalize my-3">{team?'meet our team': 'our team'}</button>


</section>

<div class="h-[200px]">
    {#if team}
    <section class="scroll-container" in:fly={{ y: -200, duration: 300, delay: 300 }}
    out:fly={{ y: 200, duration: 300 }}>
    {#each [1,1,1,1,1,1] as item}
         <div class="scroll-item text-center ">
            <img 
            src="https://c4.wallpaperflare.com/wallpaper/815/630/335/chadwick-boseman-male-celebrities-boys-hd-wallpaper-preview.jpg" 
            alt="" 
            class="w-full h-[100px] object-cover bg-gray-400 rounded-lg border-2  "/>
            <h2 class="font-bold">Black Panther</h2>
            <p class="text-">King of wakanda</p>
         </div>
    {/each}
    </section>
{/if}
</div>
<h2 class="text-xl capitalize text-center mb-4">Road map</h2>


