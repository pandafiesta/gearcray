<script>
    import GearCard from "../../components/GearCard.svelte";

    let gearList = ['Bike', 'Skis', 'Climbing Shoes']
</script>

<h1>Gear</h1>
<select name="filter" id=""><option>By sport</option></select>
<button>Share</button>
<ul>
    {#each gearList as item}
        <li>
            <GearCard name={item} />
        </li>
    {/each}
</ul>