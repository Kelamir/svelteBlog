<script>
    import { fade } from 'svelte/transition';
    let transitioning = true;

    function toggleTransition() {
        transitioning = !transitioning;
    }
</script>



<h5 transition:fade>Kelamir's blog</h5>

<ul>
    <li on:click={toggleTransition}> <a href="/">Home</a> </li>
    <li on:click={toggleTransition}> <a href="/posts">Posts</a> </li>
    <li on:click={toggleTransition}> <a href="/contact">Contact</a> </li>
    <li on:click={toggleTransition}> <a href="/about">About</a> </li>
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
