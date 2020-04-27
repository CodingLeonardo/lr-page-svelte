<script>
  export let name;
  export let src;
</script>

<style>
  .Habilidades {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    padding: 0.8em;
    border-radius: 1em;
    margin: 1em 0;
    width: 60%;
    box-shadow: 0 0 0.5em 0 black;
  }
  .Habilidades img {
    width: 100%;
  }
</style>

<div class="Habilidades">
  <img {src} alt={name} />
  <h1>{name}</h1>
</div>
