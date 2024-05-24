<div
  class="modal fade"
  id="exampleModal"
  tabindex="-1"
  aria-labelledby="exampleModalLabel"
  aria-hidden="true"
>
  <div class="modal-dialog modal-lg">
    <div class="modal-content">
      <div class="modal-header">
        <h1 class="modal-title fs-5" id="exampleModalLabel">Agregar Alumno</h1>
        <button
          type="button"
          class="btn-close"
          data-bs-dismiss="modal"
          aria-label="Close"
        ></button>
      </div>
      <div class="modal-body">
        <div class="container-fluid">
          <div class="row">
            <div class="col-2">
                <label for="cuenta" class="form-label">Cuenta</label>
                <input
                  type="text"
                  id="apellido-paterno"
                  class="form-control"
                  readonly
                />
              </div>
          </div>
          <div class="row m-0 mb-3 text-black border-bottom border-black">
            <h1 class="fs-1 titulo-filtrado mb-1">Datos del alumno</h1>
          </div>
          <div class="row">
            <div class="col">
                <label for="apellido-paterno" class="form-label"
                >Apellido Paterno</label
              >
              <input
                type="text"
                id="apellido-paterno"
                class="form-control"
              />
            </div>
            <div class="col">
                <label for="apellido-materno-agregar" class="form-label"
                >Apellido Materno</label
              >
              <input
                type="text"
                id="apellido-materno"
                class="form-control"
              />
            </div>
            <div class="col">
              <label for="nombre-alumno" class="form-label"
                >Nombre(s)</label
              >
              <input
                type="text"
                id="nombre-alumno-agregar"
                class="form-control"
              />
            </div>
            <div class="col">
                <label for="fec-nacimiento-alumnoo" class="form-label"
                  >Fecha de Nacimiento</label
                >
                <input
                  type="date"
                  id="fec-nacimiento-alumno-agregar"
                  class="form-control"
                />
              </div>
          </div>
          <div class="row"></div>
          <div class="row"></div>
          <div class="row"></div>
        </div>   
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">
          Cancelar
        </button>
        <button type="button" class="btn btn-primary">Guardar</button>
      </div>
    </div>
  </div>
</div>
