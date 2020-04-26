<script>
  export let name;
  export let src;
</script>

<style>
  .Certificado {
    width: 100%;
    border-radius: 1.5em;
    overflow: hidden;
    transition: 0.8s;
  }
  .Certificado:hover {
    z-index: 10;
    transform: scale(1.2);
  }
  .Certificado img {
    width: 100%;
  }
</style>

<div class="Certificado">
  <img {src} alt={name} />
</div>
