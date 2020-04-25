<script>
  import Navbar from "../components/Navbar.svelte";

  export let segment;
</script>

<style>
  main {
    width: 80%;
    margin: 0 auto;
  }
</style>

<main>
  <Navbar {segment} />
  <slot />
</main>
