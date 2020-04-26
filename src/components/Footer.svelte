<script>

</script>

<style>
  footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 3em;
    background: #81d878;
  }
  footer div > div {
    display: inherit;
    justify-content: center;
    align-items: center;
    font-size: 1.2em;
  }
  footer a {
    text-decoration: underline;
    color: #31522d;
  }
  img {
    height: 2em;
    margin: 0 0.5em;
  }

  @media screen and (min-width: 320px) {
    footer {
      display: flex;
      justify-content: space-evenly;
      align-items: center;
      height: 4.5em;
      flex-direction: column;
    }
    footer div > div {
      font-size: 1em;
    }
  }
  @media screen and (min-width: 768px) {
    footer {
      display: flex;
      justify-content: space-evenly;
      align-items: center;
      height: 3em;
      flex-direction: row;
    }
    footer div > div {
      font-size: 1em;
    }
  }
</style>

<footer>
  <div class="container">
    <div>
      Hecho con ❤ por
      <a href="https://github.com/CodingLeonardo">@CodingLeonardo</a>
    </div>
    <div>
      <span>Impulsado por Svelte</span>
      <img src="./assets/images/svelte.svg" alt="Svelte" />
    </div>
  </div>
</footer>
