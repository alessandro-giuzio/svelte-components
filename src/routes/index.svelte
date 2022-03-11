<script>
   import SearchFilter from "$lib/SearchFilter.svelte";
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

<SearchFilter {items} bind:search/>

{#if isToggled}
<h1>I'm Toggled!</h1>
{/if}

