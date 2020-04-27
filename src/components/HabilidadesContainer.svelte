<script>
  export let title;
  export let habilidades;
  import Habilidades from "./Habilidades.svelte";
</script>

<style>
  .HabilidadesContainer {
    display: flex;
    align-items: center;
    flex-direction: column;
    width: 100%;
    box-shadow: 0 0 10px 0 black;
    background: white;
    border-radius: 2em;
    padding: 1em;
    text-align: center;
    margin: 1em 0;
  }
  .HabilidadesContainer h1 {
    margin-bottom: 0.5em;
  }
</style>

<div class="HabilidadesContainer">
  <h1>{title}</h1>
  {#each habilidades as habilidad}
    <Habilidades name={habilidad.name} src={habilidad.src} />
  {/each}
</div>
