<script>
    import Toggle from "$lib/Toggle.svelte";
    let isToggled = false;
</script>

<h1>Alessandro's Components</h1>

<Toggle bind:isToggled label="Beta User" />
<Toggle bind:isToggled label="Beta User" style="--toggle-background-color:red"/>

{#if isToggled}
<h1>I'm Toggled!</h1>
{/if}

