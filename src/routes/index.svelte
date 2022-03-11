<script>
   import SearchFilter from "$lib/SearchFilter.svelte";
   import Field from "$lib/Field.svelte";
    let isToggled = false;
    let items = [
        'Alessandro',
        'Oihana',
        'Luca',
        'Maria',
        'Haizea',
        'rosarito',
    ]
    let search = '';
</script>

<h1>Alessandro's Components {search}</h1>

<Field bind:value={search} label="Search" instructions="Type to search" placeholder="Ale" />
<Field value=0 label="Number" type="number"  />

<SearchFilter {items} bind:search/>

{#if isToggled}
<h1>I'm Toggled!</h1>
{/if}

