<script>
  import HabilidadesContainer from "../components/HabilidadesContainer.svelte";

  const lenguages = [
    { name: "Html", src: "./assets/images/html5.svg" },
    { name: "CSS", src: "./assets/images/css3.svg" },
    { name: "Javascript", src: "./assets/images/javascript.svg" }
  ];

  const frameworks = [
    { name: "ReactJS", src: "./assets/images/react.svg" },
    { name: "NextJS", src: "./assets/images/nextjs.svg" },
    { name: "Svelte", src: "./assets/images/svelte.svg" },
    { name: "Sapper", src: "./assets/images/nextjs.svg" },
    { name: "NodeJS", src: "./assets/images/nodejs.svg" }
  ];

  const devtools = [
    { name: "Webpack", src: "./assets/images/webpack.svg" },
    { name: "PostCSS", src: "./assets/images/postcss.svg" },
    { name: "Git", src: "./assets/images/git.svg" }
  ];

  const consultdatas = [
    { name: "GraphQL", src: "./assets/images/graphql.svg" }
  ];
</script>

<style>
  .Habilidades {
    width: 100%;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(2, 1fr);
    gap: 1.5em;
  }
  @media screen and (min-width: 320px) {
    .Habilidades {
      grid-template-columns: 1fr;
      grid-template-rows: initial;
    }
  }
  @media screen and (min-width: 425px) {
    .Habilidades {
      grid-template-columns: repeat(2, 1fr);
      grid-template-rows: repeat(2, 1fr);
    }
  }
</style>

<svelte:head>
  <title>Leonardo Rivero - Desarrollador Frontend</title>
</svelte:head>

<div class="Habilidades">
  <HabilidadesContainer title="Lenguajes" habilidades={lenguages} />
  <HabilidadesContainer
    title="Frameworks y Librerias"
    habilidades={frameworks} />
  <HabilidadesContainer
    title="Herramientas de desarrollo"
    habilidades={devtools} />
  <HabilidadesContainer title="Consulta de Datos" habilidades={consultdatas} />
</div>
