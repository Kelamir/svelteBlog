<script>
  import "../app.css";
</script>

<h2 class="text-2xl font-bold underline first-letter:text-6xl first-letter:font-bold">Kelamir's blog</h2>

<div class="grid grid-cols-5 w-1/4 p-3">
  <a class="border bg-gray-300 text-zink-300 hover:text-zink-700 text-center hover:animate-spin" href="/">Home</a>
  <a class="border bg-gray-300 text-zink-300 hover:text-zink-700 text-center hover:animate-ping" href="/posts">Posts</a>
  <a class="border bg-gray-300 text-zink-300 hover:text-zink-700 text-center hover:animate-pulse" href="/contact">Contact</a>
  <a class="border bg-gray-300 text-zink-300 hover:text-zink-700 text-center hover:animate-bounce" href="/about">About</a>

</div>

<slot class="mx self-center"/>

<style lang="postcss">
  :global(html) {
    background-color: theme(colors.indigo.100);
  }
</style>