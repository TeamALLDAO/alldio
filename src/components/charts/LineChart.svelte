<script>
// @ts-nocheck

    import Chart from 'svelte-frappe-charts';

    const data = {
    labels: [ "july 1st", "july 7th", "july 14th", "july 21th",
        "july 28th", "31st", 
    ],
    datasets: [
       
        {
            
            values: [ 200, 300, 250, 800, 400, 300, 500, 340, 250]
        }
    ]
}

</script>






<Chart data={data} type="line" />

<div id="chart"></div>