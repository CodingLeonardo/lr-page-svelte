<script>
  import Socialbar from "./Socialbar.svelte";
  export let segment;
</script>

<style>
  header {
    /* background: #a5ff9b; */
    padding-top: 0.5em;
  }
  header > div {
    text-align: center;
  }
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
    color: #56a34d;
    padding: 1em 0.5em;
    display: block;
    transition: 0.8s;
    will-change: color;
  }
  a:hover {
    color: #20421d;
  }

  .About {
    display: flex;
    align-items: center;
    flex-direction: column;
    text-align: center;
    color: black;
    padding: 1em 2em;
    /* background: #a5ff9b; */
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
</style>

<header>

  <div>
    <div class="About">
      <figure class="About-perfile">
        <a href="/">
          <img src="./assets/images/Leonardito.jpg" alt="Leonardo Rivero" />

        </a>
      </figure>
      <div class="About-info">
        <h1>Leonardo Rivero</h1>
        <span>Desarrollador Frontend</span>
      </div>
    </div>
  </div>
  <Socialbar />
  <nav>
    <ul>
      <li>
        <a href="/certificados">Certificados</a>
      </li>
      <li>
        <a href="/habilidades">Habilidades</a>
      </li>
    </ul>
  </nav>

</header>
