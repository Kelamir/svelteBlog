<script>
  import "../app.css";
</script>

<h2 class="text-2xl font-bold underline">Kelamir's blog</h2>

<nav>
    <a href="/">Home</a>
    <a href="/posts">Posts</a>
    <a href="/contact">Contact</a>
    <a href="/about">About</a>
</nav>

<slot />


<style lang="postcss">
  :global(html) {
    background-color: theme(colors.gray.100);
  }
</style>