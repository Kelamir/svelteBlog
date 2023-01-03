<script>
    import { fade } from 'svelte/transition';
    let visible = true;
</script>



<input type="checkbox" bind:checked={visible}>


{#if visible}
    <h5 transition:fade>Kelamir's blog</h5>

    <ul transition:fade>
        <li> <a href="/home">Home</a> </li>
        <li> <a href="/posts">Posts</a> </li>
        <li> <a href="/contact">Contact</a> </li>
        <li> <a href="/about">About</a> </li>
    </ul>
{/if}

<slot />


<style>
    ul { display: flex; flex-direction: row}
    li { display: flex;  margin-left: 5px}

</style>
