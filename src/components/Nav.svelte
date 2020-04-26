<script>
  export let links;
</script>

<style>
  nav {
    display: flex;
    justify-content: center;
    border-bottom: 0.2em solid var(--primary-500);
    font-weight: normal;
  }

  ul {
    margin: 0;
    padding: 0;
  }

  /* clearfix */
  ul::after {
    content: "";
    display: block;
    clear: both;
  }

  li {
    display: block;
    float: left;
  }
  a {
    text-decoration: none;
    color: #45853e;
    font-size: 1.2em;
    padding: 1em 0.5em;
    display: block;
    transition: 0.8s;
    will-change: color;
  }
  a:hover {
    color: #183116;
  }
</style>

<nav>
  <ul>
    {#each links as link}
      <li>
        <a href={`${link.href}`}>{link.name}</a>
      </li>
    {/each}
  </ul>
</nav>
