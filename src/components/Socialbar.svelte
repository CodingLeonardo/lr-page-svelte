<script>
  export let links;
</script>

<style>
  .Socialbar {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 3em;
    margin: 1em 0;
  }
  .Socialbar div {
    width: 10%;
    margin: 0 0.25em;
  }
  .Socialbar img {
    width: 100%;
  }
  @media screen and (min-width: 320px) {
    .Socialbar div {
      width: 15%;
    }
  }
  @media screen and (min-width: 768px) {
    .Socialbar div {
      width: 10%;
    }
  }
  @media screen and (min-width: 1024px) {
    .Socialbar div {
      width: 8%;
    }
  }
  @media screen and (min-width: 1440px) {
    .Socialbar div {
      width: 5%;
    }
  }
  @media screen and (min-width: 2560px) {
    .Socialbar div {
      width: 2%;
    }
  }
</style>

<div class="Socialbar">
  {#each links as link}
    <div>
      <a href={link.href} target="_blank">
        <img src={link.src} alt={link.name} />
      </a>
    </div>
  {/each}
</div>
