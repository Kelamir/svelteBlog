<script>
    import { fade } from 'svelte/transition';
    let transitioning = true;
</script>



<input type="checkbox" bind:checked={transitioning}>

    <h5 transition:fade>Kelamir's blog</h5>

    <ul>
        <li on:click={transitioning = !transitioning}> <a href="/home">Home</a> </li>
        <li on:click={transitioning = !transitioning}> <a href="/posts">Posts</a> </li>
        <li on:click={transitioning = !transitioning}> <a href="/contact">Contact</a> </li>
        <li on:click={transitioning = !transitioning}> <a href="/about">About</a> </li>
    </ul>

{#if transitioning}
    <div transition:fade>
        <slot />
    </div>
{/if}

<style>
    ul { display: flex; flex-direction: row}
    li { display: flex;  margin-left: 5px}

</style>
