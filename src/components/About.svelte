<script>
  export let name;
  export let ocupation;
  export let srcImg;
  export let href;
</script>

<style>
  .About {
    display: flex;
    align-items: center;
    flex-direction: column;
    text-align: center;
    color: black;
    padding: 1em 2em;
  }
  .About-perfile {
    width: 50%;
  }
  .About-perfile img {
    width: 100%;
    border-radius: 50%;
    box-shadow: 0 0 1em black;
  }
  .About-info {
    margin-top: 0.5em;
  }
  .About a {
    padding: 0;
    color: #20421d;
  }
  .About-info h1 {
    font-weight: lighter;
  }
  .About-info span {
    font-weight: lighter;
    font-size: 1.1em;
  }
  @media screen and (min-width: 320px) {
    .About-info h1 {
      font-size: 1.8em;
    }
    .About-info {
      margin-top: 0.8em;
    }
  }
  @media screen and (min-width: 768px) {
    .About-info h1 {
      font-size: 2.5em;
    }
    .About-info {
      margin-top: 0.8em;
    }
  }
</style>

<div class="About">
  <figure class="About-perfile">
    <a {href}>
      <img src={srcImg} alt={name} />
    </a>
  </figure>
  <div class="About-info">
    <h1>{name}</h1>
    <span>{ocupation}</span>
  </div>
</div>
