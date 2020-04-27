<script>
  export let name;
  export let src;
  export let background;
</script>

<style>
  .Habilidad {
    position: relative;
    width: 12em;
    padding: 1em;
    background-color: #a5ff9b;
    box-shadow: 0 0 0.2em 0 black;
    border-radius: 1em;
    margin: 0 1em;
    overflow: hidden;
    transition: 0.7s;
  }
  .Habilidad header {
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    background: #f1652a;
    height: 8em;
    margin: -20px -20px 20px -20px;
    overflow: hidden;
  }
  .Habilidad-image {
    position: absolute;
    display: block;
    width: 5em;
    height: 5em;
    transition: 0.7s;
  }
  .Habilidad-title {
    height: 40px;
    overflow: hidden;
  }

  .Habilidad-title p {
    font-size: 1.5em;
    text-transform: uppercase;
    font-weight: bold;
  }

  .Habilidad:hover {
    transform: scale(1.2);
    z-index: 10;
  }
  .Habilidad:hover .Habilidad-image {
    width: 10em;
    height: 10em;
  }
  @media screen and (min-width: 320px) {
    .Habilidad {
      margin: 1em 0;
    }
  }
  @media screen and (min-width: 1024px) {
    .Habilidad {
      margin: 1em;
    }
  }
</style>

<div class="Habilidad">
  <header style={`background: ${background}`}>
    <img class="Habilidad-image" {src} alt={name} />
  </header>
  <div class="Habilidad-title">
    <p>{name}</p>
  </div>
</div>
