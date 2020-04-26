<script>
  export let certificados;
  import Certificado from "./Certificado.svelte";
</script>

<style>
  .CertificadosContainer {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 1em;
    padding: 1em 0;
  }
</style>

<div class="CertificadosContainer">
  {#each certificados as certificado}
    <Certificado src={certificado.src} name={certificado.name} />
  {/each}
</div>
