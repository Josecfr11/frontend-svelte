<script>
    import logoArteCuliacan from "$lib/images/arteculiacan-modified.png";
</script>

<div class="d-flex flex-column my-2 flex-shrink-0 sidebar shadow rounded">
  <a
    href="/"
    class="d-flex align-items-center mb-3 mb-md-0 me-md-auto link-body-emphasis text-decoration-none"
  >
    <div class="vstack gap-2">
      <img
        class="img-fluid w-75 align-self-center pt-3"
        src={logoArteCuliacan}
        alt="imagen_logo_arteculiacan"
      />
      <span id="titulo-sidebar" class="titulo-sidebar align-self-center"
        >Arte Culiacan</span
      >
    </div>
  </a>
  <hr />
  <ul class="nav nav-pills flex-column mb-auto align-items-center">
    <li class="nav-item">
      <a class="icon-link icon-link-hover btn" href="/alumnos">
        <i class="fas fa-graduation-cap"></i>
        Alumnos
      </a>
    </li>
    <li class="nav-item align-content-center">
      <a class="icon-link icon-link-hover btn" href="/recibos">
        <i class="fa-solid fa-file-invoice-dollar"></i>
        Recibos
      </a>
    </li>
  </ul>
  <hr />
</div>

<style>
  .sidebar {
    background-color: #dcd3ce;
    width: 10vw;
  }

  .titulo-sidebar {
    font-size: 1em;
  }
</style>
