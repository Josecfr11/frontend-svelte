
<script>
    import ModalAgregarAlumno from "./ModalAgregarAlumno.svelte";
    import "bootstrap/dist/js/bootstrap.bundle.min.js";
</script>

<div class="container-fluid my-2 main-content-alumnos">
    <div class="row m-0 mb-3 text-black border-bottom border-black">
      <h1 class="titulo-filtrado mb-1">Filtrado de Alumnos</h1>
    </div>
    <form action="/index">
      <div class="row m-0">
        <div class="col-3">
          <label for="apellido-paterno" class="form-label"
            >Apellido Paterno</label
          >
          <input type="text" id="apellido-paterno-filtrado" class="form-control" />
        </div>
        <div class="col-3">
          <label for="apellido-materno" class="form-label"
            >Apellido Materno</label
          >
          <input type="text" id="apellido-materno-filtrado" class="form-control" />
        </div>
        <div class="col-4">
          <label for="nombre-alumno-filtrado" class="form-label"
            >Nombre(s)</label
          >
          <input
            type="text"
            id="nombre-alumno-filtrado"
            class="form-control"
          />
        </div>
        <div class="vertical-end col-2">
          <button
            type="submit"
            class="btn border-4 btn-outline-primary w-100"
          >
            Buscar
            <i class="fa-solid fa-magnifying-glass"></i>
          </button>
          
        </div>
      </div>
    </form>
    <hr />
    <div class="container-fluid">
      <div class="row">
        <div class="col-2 mb-1">
          <button
            type="button"
            class="btn border-4 btn-outline-primary"
            data-bs-toggle="modal"
            data-bs-target="#exampleModal"
          >
            Agregar alumno
            <i class="fa-solid fa-user-plus"></i>
          </button>
        </div>
        <ModalAgregarAlumno/>
      </div>


      <div class="row">
        <table class="table table-hover">
          <thead>
            <tr>
              <th scope="col">Cuenta</th>
              <th scope="col">Apellidos</th>
              <th scope="col">Nombre</th>
              <th scope="col">Taller</th>
              <th scope="col">Horario</th>
              <th scope="col">Grupo</th>
              <th scope="col">Acciones</th>
            </tr>
          </thead>
          <tbody class="table-group-divider">
            <tr>
              <th scope="row">1</th>
              <td>Gastelum Astoga</td>
              <td>Monserrat</td>
              <td>Dibujo y Pintura Infantil</td>
              <td>Sabatinos Matutino</td>
              <td>Grupo 2</td>
              <td>
                <div class="container-fluid">
                  <div class="row">
                    <div class="col">
                      <button
                        type="button"
                        class="btn btn-warning w-100"
                        data-bs-toggle="tooltip"
                        data-bs-placement="top"
                        data-bs-title="Editar"
                      >
                        <i class="fa-regular fa-pen-to-square"></i>
                      </button>
                    </div>
                    <div class="col">
                      <button
                        type="button"
                        class="btn btn-danger w-100"
                        data-bs-toggle="tooltip"
                        data-bs-placement="top"
                        data-bs-original-title="Eliminar"
                      >
                        <i class="fa-solid fa-trash-can"></i>
                      </button>
                    </div>
                    <div class="col">
                      <button
                        type="button"
                        class="btn btn-info w-100"
                        data-bs-toggle="tooltip"
                        data-bs-placement="top"
                        data-bs-title="Información"
                      >
                        <i class="fa-solid fa-circle-info"></i>
                      </button>
                    </div>
                    <div class="col">
                      <button
                        type="button"
                        class="btn btn-secondary w-100"
                        data-bs-toggle="tooltip"
                        data-bs-placement="top"
                        data-bs-title="Historial"
                      >
                        <i class="fa-solid fa-book-open"></i>
                      </button>
                    </div>
                  </div>
                </div>
              </td>
            </tr>
            <tr>
              <th scope="row">2</th>
              <td>Jacob</td>
              <td>Thornton</td>
              <td>@fat</td>
            </tr>
            <tr>
              <th scope="row">3</th>
              <td colspan="2">Larry the Bird</td>
              <td>@twitter</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>

<style>
  .main-content-alumnos {
    width: 90vw;
  }

  .titulo-filtrado {
    font-size: 2em;
  }

  .vertical-end {
    display: flex;
    align-items: end;
    justify-content: center;
  }


</style>
