<script>
  import HabilidadesContainer from "../components/HabilidadesContainer.svelte";

  const lenguages = [
    { name: "Html", src: "./assets/images/html5.svg", background: "#F1652A" },
    { name: "CSS", src: "./assets/images/css3.svg", background: "#2965F1" },
    {
      name: "Javascript",
      src: "./assets/images/javascript.svg",
      background: "#C2B140"
    }
  ];

  const frameworks = [
    {
      name: "ReactJS",
      src: "./assets/images/react.svg",
      background: "#151515"
    },
    {
      name: "NextJS",
      src: "./assets/images/nextjs.svg",
      background: "#F8F8F8"
    },
    {
      name: "Svelte",
      src: "./assets/images/svelte.svg",
      background: "#F8F8F8"
    },
    {
      name: "Sapper",
      src: "./assets/images/sapper.svg",
      background: "#F8F8F8"
    },
    { name: "NodeJS", src: "./assets/images/nodejs.svg", background: "#8DBF3F" }
  ];

  const devtools = [
    {
      name: "Webpack",
      src: "./assets/images/webpack.svg",
      background: "#8AD0F4"
    },
    {
      name: "PostCSS",
      src: "./assets/images/postcss.svg",
      background: "#F8F8F8"
    },
    { name: "Git", src: "./assets/images/git.svg", background: "#F8F8F8" }
  ];

  const consultdatas = [
    {
      name: "GraphQL",
      src: "./assets/images/graphql.svg",
      background: "#151E25"
    }
  ];
</script>

<style>
  .Habilidades {
    width: 100%;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(2, 1fr);
    padding-bottom: 1.5em;
    gap: 1.5em;
  }

  h1 {
    text-align: center;
    font-size: 2.8em;
    margin: 0.5em 0;
    font-family: "Source Sans Pro";
    text-transform: uppercase;
    font-weight: 400;
  }

  @media screen and (min-width: 320px) {
    .Habilidades {
      grid-template-columns: 1fr;
      grid-template-rows: initial;
    }
  }
  @media screen and (min-width: 768px) {
    .Habilidades {
      grid-template-columns: repeat(2, 1fr);
      grid-template-rows: repeat(2, 1fr);
    }
  }
  @media screen and (min-width: 1024px) {
    .Habilidades {
      grid-template-columns: initial;
      grid-template-rows: repeat(4, 1fr);
    }
  }
</style>

<svelte:head>
  <title>Leonardo Rivero - Desarrollador Frontend</title>
</svelte:head>

<h1>Habilidades</h1>

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
