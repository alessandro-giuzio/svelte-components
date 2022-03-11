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
</script>

<h1>Alessandro's Components</h1>

<SearchFilter {items} />
<!-- <BetterAccordion isOpen={true} buttonText = "Do I need it?" >
<div>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam illum fugit tenetur deserunt nemo minus dolorum, quaerat ad quae. Aperiam doloremque veniam in quisquam laudantium.</p>
</div>
</BetterAccordion> -->
<!-- <Toggle bind:isToggled label="Beta User" />
<Toggle bind:isToggled label="Beta User" style="--toggle-background-color:red"/>
 -->
{#if isToggled}
<h1>I'm Toggled!</h1>
{/if}

