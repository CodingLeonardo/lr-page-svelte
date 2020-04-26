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
