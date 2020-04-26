<script>
  import Navbar from "../components/Navbar.svelte";
  import Footer from "../components/Footer.svelte";

  export let segment;
</script>

<style>
  main {
    width: 80%;
    margin: 0 auto;
  }
</style>

<Navbar {segment} />
<main>
  <slot />
</main>
<Footer />
