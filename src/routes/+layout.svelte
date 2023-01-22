<script>
  import "../app.css";
</script>


<div class="flex justify-center">
  <h2 class="text-2xl font-bold underline">Kelamir's blog</h2>
  <nav>
      <a href="/">Home</a>
      <a href="/posts">Posts</a>
      <a href="/contact">Contact</a>
      <a href="/about">About</a>
  </nav>
<slot class="mx self-center"/>
</div>



<style lang="postcss">
  :global(html) {
    background-color: theme(colors.yellow.100);
  }
</style>