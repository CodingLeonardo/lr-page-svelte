<script>
  const links = [
    {
      name: "facebook",
      src: "./assets/images/facebook.svg",
      href: "https://www.facebook.com/CodingLeonardo"
    },
    {
      name: "twitter",
      src: "./assets/images/twitter.svg",
      href: "https://twitter.com/CodingLeonardo"
    },
    {
      name: "instagram",
      src: "./assets/images/instagram.svg",
      href: "https://www.instagram.com/codingleonardo/"
    },
    {
      name: "github",
      src: "./assets/images/github.svg",
      href: "https://github.com/CodingLeonardo"
    }
  ];
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
