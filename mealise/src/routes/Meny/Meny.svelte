<script>
	import MenyItem from "./MenyItem.svelte";

    let menuItems = [
        {id:1,titel:"Besök skogen", link:"skogen"},
        {id:2,titel:"Hitta maträtter", link:""},
        {id:3,titel:"Inställningar", link:""}   
    ];
</script>
<ul>
    {#each menuItems as Item}
        <MenyItem text={Item.titel}></MenyItem>
    {/each}
</ul>