<script>
  import Navbar from "../components/Navbar.svelte";
  import AboutBar from "../components/AboutBar.svelte";

  export let segment;
</script>

<style>
  main {
    display: grid;
    grid-template-columns: minmax(150px, 400px) 1fr;
  }
</style>

<Navbar {segment} />
<main>
  <div>
    <AboutBar
      name="Leonardo Rivero"
      src="./assets/images/Leonardito.jpg"
      ocupation="Desarrollador Frontend"
      bio="Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus
      veniam sapiente vitae molestiae ea itaque commodi, corrupti aliquam!
      Aspernatur, commodi. Ad laborum ipsum fugiat magnam mollitia? Fuga
      possimus ab harum non praesentium quibusdam doloremque! Eaque, voluptatem?
      Fugiat itaque sapiente quasi esse tenetur inventore recusandae incidunt,
      veritatis omnis sunt ex reprehenderit?"
      live="Caracas, Venezuela" />
  </div>
  <div>
    <slot />
  </div>
</main>
