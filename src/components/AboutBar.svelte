<script>
  export let src;
  export let name;
  export let ocupation;
  export let bio;
  export let live;
</script>

<style>
  .AboutBar {
    display: flex;
    align-items: center;
    flex-direction: column;
    padding: 2em 1em;
    text-align: center;
  }
  .AboutBar-perfile {
    width: 80%;
  }
  .AboutBar-perfile img {
    width: 100%;
    border-radius: 50%;
    border: 0.2em solid var(--primary-300);
    box-shadow: 0 0 0.5em black;
  }
  .AboutBar-info {
    margin-top: 1em;
  }
  .AboutBar-info h1 {
    font-weight: lighter;
  }
  .AboutBar-info span {
    font-weight: lighter;
    font-size: 1.1em;
  }
  .AboutBar-bio {
    margin: 1em 0;
    color: #8a8a8a;
    font-weight: lighter;
  }
  .AboutBar-live {
    color: #646464;
    font-weight: lighter;
    font-size: 1.1em;
  }
</style>

<div class="AboutBar">
  <figure class="AboutBar-perfile">
    <img {src} alt={name} />
  </figure>
  <div class="AboutBar-info">
    <h1>{name}</h1>
    <span>{ocupation}</span>
  </div>
  <div class="AboutBar-bio">
    <p>{bio}</p>
  </div>
  <div class="AboutBar-live">
    <p>{live}</p>
  </div>
</div>
