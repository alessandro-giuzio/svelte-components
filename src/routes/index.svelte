<script>
    import Toggle from "$lib/Toggle.svelte";
    import BetterAccordion from "$lib/BetterAccordion.svelte";
    let isToggled = false;
</script>

<h1>Alessandro's Components</h1>
<BetterAccordion isOpen={true} buttonText = "Do I need it?" >
<div>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Magnam illum fugit tenetur deserunt nemo minus dolorum, quaerat ad quae. Aperiam doloremque veniam in quisquam laudantium.</p>
</div>
</BetterAccordion>
<Toggle bind:isToggled label="Beta User" />
<Toggle bind:isToggled label="Beta User" style="--toggle-background-color:red"/>

{#if isToggled}
<h1>I'm Toggled!</h1>
{/if}

