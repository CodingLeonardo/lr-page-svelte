<script>
  export let segment;
</script>

<style>
  nav {
    display: flex;
    justify-content: center;
    border-bottom: 1px solid var(--primary-100);
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

  [aria-current] {
    position: relative;
    display: inline-block;
  }

  [aria-current]::after {
    position: absolute;
    content: "";
    width: calc(100% - 1em);
    height: 2px;
    background-color: rgb(255, 62, 0);
    display: block;
    bottom: -1px;
  }

  a {
    text-decoration: none;
    color: rgb(77, 77, 77);
    padding: 1em 0.5em;
    display: block;
    transition: 0.8s;
    will-change: color;
  }

  a:hover {
    color: black;
  }
</style>

<div />

<nav>
  <ul>
    <li>
      <a
        aria-current={segment === 'certificados' ? 'page' : undefined}
        href="/certificados">
        Certificados
      </a>
    </li>
    <li>
      <a
        aria-current={segment === 'habilidades' ? 'page' : undefined}
        href="/habilidades">
        Habilidades
      </a>
    </li>
  </ul>
</nav>
