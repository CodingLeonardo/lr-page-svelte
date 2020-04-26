<script>
  import CertificadosContainer from "../components/CertificadosContainer.svelte";
</script>

<style>
  h1 {
    text-align: center;
    margin: 0.5em 0;
    font-size: 2.8em;
  }
</style>

<svelte:head>
  <title>Leonardo Rivero - Desarrollador Frontend</title>
</svelte:head>

<h1>Certificados</h1>

<div class="Certificados">
  <CertificadosContainer
    certificados={[{ name: 'Programacion Basica', src: '../assets/images/diploma-programacion-basica.svg', categories: ['Programacion', 'Todos'] }, { name: 'Marca Personal', src: '../assets/images/diploma-marca-personal.svg', categories: ['Marketing', 'Todos'] }, { name: 'Desarrollo Web Online', src: '../assets/images/diploma-html5-css3.svg', categories: ['Programacion', 'Todos'] }, { name: 'Responsive Design', src: '../assets/images/diploma-responsive-design.svg', categories: ['Programacion', 'Todos'] }, { name: 'Git y Github', src: '../assets/images/diploma-git-github.svg', categories: ['Programacion', 'Todos'] }, { name: 'CSS Grid Layout', src: '../assets/images/diploma-css-grid-layout.svg', categories: ['Programacion', 'Todos'] }, { name: 'Fundamentos de Javascript', src: '../assets/images/diploma-fundamentos-javascript.svg', categories: ['Programacion', 'Todos'] }, { name: 'Ecmascipt 6+', src: '../assets/images/diploma-ecmascript-6.svg', categories: ['Programacion', 'Todos'] }, { name: 'Motor V8 de Chrome', src: '../assets/images/diploma-javascript-navegador.svg', categories: ['Programacion', 'Todos'] }, { name: 'Javacript Profesional', src: '../assets/images/diploma-javascript-profesional.svg', categories: ['Programacion', 'Todos'] }, { name: 'SPA Javacript', src: '../assets/images/diploma-spa-javascript.svg', categories: ['Programacion', 'Todos'] }, { name: 'Webpack', src: '../assets/images/diploma-webpack.svg', categories: ['Programacion', 'Todos'] }, { name: 'PostCSS', src: '../assets/images/diploma-postcss.svg', categories: ['Programacion', 'Todos'] }, { name: 'Animaciones Web', src: '../assets/images/diploma-animaciones-web.svg', categories: ['Programacion', 'Todos'] }, { name: 'Prework', src: '../assets/images/diploma-prework.svg', categories: ['Programacion', 'Todos'] }, { name: 'React', src: '../assets/images/diploma-react.svg', categories: ['Programacion', 'Todos'] }, { name: 'React Router y Redux', src: '../assets/images/diploma-react-router-redux.svg', categories: ['Programacion', 'Todos'] }, { name: 'NextJS', src: '../assets/images/diploma-next-js.svg', categories: ['Programacion', 'Todos'] }, { name: 'GraphQL', src: '../assets/images/diploma-graphql.svg', categories: ['Programacion', 'Todos'] }, { name: 'TailwindCSS', src: '../assets/images/diploma-tailwind-css.svg', categories: ['Programacion', 'Todos'] }, { name: 'Backend con NodeJS', src: '../assets/images/diploma-backend-js.svg', categories: ['Programacion', 'Todos'] }, { name: 'Hablar en Publico', src: '../assets/images/diploma-hablar-en-publico.svg', categories: ['CrecimientoProfesional', 'Todos'] }, { name: 'Storytelling', src: '../assets/images/diploma-storytelling.svg', categories: ['CrecimientoProfesional', 'Todos'] }, { name: 'Arquitecto Frontend', src: '../assets/images/diploma-arquitecto.svg', categories: ['Programacion', 'Todos'] }]} />
</div>
