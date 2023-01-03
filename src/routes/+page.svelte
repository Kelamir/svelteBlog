<script>
    export let data;
</script>

<h1>Kelamir's blog</h1>

<ul>
    {#each data.summaries as { slug, title}}
        <li><a href="/{slug}">{title}</a></li>
    {/each}
</ul>