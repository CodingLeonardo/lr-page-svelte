<script>
  import About from "./About.svelte";
  import Socialbar from "./Socialbar.svelte";
  import Nav from "./Nav.svelte";
</script>

<style>
  header {
    padding-top: 0.5em;
  }
</style>

<header>
  <div class="container">
    <About
      name="Leonardo Rivero"
      ocupation="Desarrollador Frontend"
      srcImg="./assets/images/Leonardito.jpg"
      href="/" />
    <Socialbar
      links={[{ name: 'facebook', src: './assets/images/facebook.svg', href: 'https://www.facebook.com/CodingLeonardo' }, { name: 'twitter', src: './assets/images/twitter.svg', href: 'https://twitter.com/CodingLeonardo' }, { name: 'instagram', src: './assets/images/instagram.svg', href: 'https://www.instagram.com/codingleonardo/' }, { name: 'github', src: './assets/images/github.svg', href: 'https://github.com/CodingLeonardo' }]} />
    <Nav
      links={[{ name: 'Certificados', href: '/certificados' }, { name: 'Habilidades', href: '/habilidades' }]} />
  </div>
</header>
