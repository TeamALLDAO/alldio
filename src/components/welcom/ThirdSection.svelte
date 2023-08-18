<script>
    const info = [
        {
            name:"DSMD",
            text:"AllDao offers institutional-grade Polygon infrastructure, on-chain data and staking services, Faster transactions and lower fees makes interactions with Alldao on polygon perfect. Being a full part of the Polygon Ecosystem, coming into contact with communities, developers, professionals and projects."
        },
        {
            name:"DI",
            text:`DI means Decentralized Investment DAO DI is a DAO focused on making decentralized investments in early-stage blockchain projects. Members can submit investment proposals and vote on which projects to invest in.`
        },
        {
            name:"DSMD",
            text:"AllDao offers institutional-grade Polygon infrastructure, on-chain data and staking services, Faster transactions and lower fees makes interactions with Alldao on polygon perfect. Being a full part of the Polygon Ecosystem, coming into contact with communities, developers, professionals and projects."
        },
        {
            name:"DI",
            text:`DI means Decentralized Investment DAO DI is a DAO focused on making decentralized investments in early-stage blockchain projects. Members can submit investment proposals and vote on which projects to invest in.`
        },
        {
            name:"DSMD",
            text:"AllDao offers institutional-grade Polygon infrastructure, on-chain data and staking services, Faster transactions and lower fees makes interactions with Alldao on polygon perfect. Being a full part of the Polygon Ecosystem, coming into contact with communities, developers, professionals and projects."
        },
        {
            name:"DI",
            text:`DI means Decentralized Investment DAO DI is a DAO focused on making decentralized investments in early-stage blockchain projects. Members can submit investment proposals and vote on which projects to invest in.`
        }
    ];
</script>


<div class="my-4">
    <div class="flex justify-between items-center my-4">
        <h2 class="text-2xl font-bold">Explore Daos</h2>
        <button class="text-[#FF4D4D]">See All</button>
    </div>


    <div class=" grid gap-4 grid-cols-3 ">
       {#each info  as inf, index }
       <div class="  mb-4  bg-white p-4 first-letter inline-block gap-3 rounded-lg">
            <div class="font-bold mb-2 text-3xl w-[50px] bg-black rounded-full h-[50px] grid text-white place-content-center">{index+1}</div>
            <h2 class="mb-2 font-bold">{inf.name}</h2>
            <p>{inf.text}</p>
        </div>
       {/each}
    </div>
</div>