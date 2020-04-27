<script>
  export let name;
  export let src;
  import IntersectionObserver from "./IntersectionObserver.svelte";
  import Loader from "./Loader.svelte";
</script>

<style>
  .Certificado {
    width: 100%;
    border-radius: 1.5em;
    overflow: hidden;
    transition: 0.8s;
  }
  .Certificado:hover {
    z-index: 10;
    transform: scale(1.2);
  }
  .Certificado img {
    width: 100%;
  }
</style>

<IntersectionObserver let:intersecting once={true} bottom={100}>
  {#if intersecting}
    <div class="Certificado">
      <img {src} alt={name} />
    </div>
  {:else}
    <Loader style="width: 100%, height: 100%" />
  {/if}
</IntersectionObserver>
