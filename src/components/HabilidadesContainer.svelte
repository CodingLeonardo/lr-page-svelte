<script>
  export let title;
  export let habilidades;
  import Habilidad from "./Habilidad.svelte";
</script>

<style>
  .HabilidadesContainer {
    display: flex;
    align-items: center;
    flex-direction: column;
    width: 100%;
    background: #81d878;
    border-radius: 2em;
    padding: 1em;
    text-align: center;
  }
  .HabilidadesContainer-container {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
  }
  .HabilidadesContainer h1 {
    margin: 0.5em 0;
  }

  @media screen and (min-width: 320px) {
    .HabilidadesContainer-container {
      flex-direction: column;
    }
  }
  @media screen and (min-width: 1024px) {
    .HabilidadesContainer h1 {
      font-size: 2.3em;
    }
    .HabilidadesContainer-container {
      flex-direction: row;
    }
  }
</style>

<div class="HabilidadesContainer">
  <h1>{title}</h1>
  <div class="HabilidadesContainer-container">
    {#each habilidades as habilidad}
      <Habilidad
        name={habilidad.name}
        src={habilidad.src}
        background={habilidad.background} />
    {/each}
  </div>
</div>
