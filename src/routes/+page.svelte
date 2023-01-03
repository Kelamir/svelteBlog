<script>
    export let data;
</script>

<ul>
    {#each data.summaries as { slug, title}}
        <li><a href="/{slug}">{title}</a></li>
    {/each}
</ul>