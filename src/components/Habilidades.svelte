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
  .Habilidades h1 {
    margin-top: 0.5em;
  }
  @media screen and (min-width: 320px) {
    .Habilidades {
      width: 60%;
    }
    .Habilidades img {
      width: 70%;
    }
    .Habilidades h1 {
      font-size: 1.5em;
    }
  }
  @media screen and (min-width: 425px) {
    .Habilidades {
      width: 80%;
    }
    .Habilidades img {
      width: 80%;
    }
    .Habilidades h1 {
      font-size: 1.3em;
    }
  }
  @media screen and (min-width: 768px) {
    .Habilidades {
      width: 50%;
    }
    .Habilidades img {
      width: 80%;
    }
    .Habilidades h1 {
      font-size: 1.4em;
    }
  }
  @media screen and (min-width: 1024px) {
    .Habilidades {
      width: 50%;
    }
    .Habilidades img {
      width: 80%;
    }
    .Habilidades h1 {
      font-size: 1.4em;
    }
  }
</style>

<div class="Habilidades">
  <img {src} alt={name} />
  <h1>{name}</h1>
</div>
