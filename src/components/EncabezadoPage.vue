<template>
<div>
          <div class="row">
            <nav class="nav-list col-md-12 "></nav>                
                <div class="col-md-7">
                    <h2 class="h2 text-center text-light">SEMANA 2</h2> 
                </div>

                <div class="col-md-4">
                    <ul class="nav justify-content-end ">
                        <li class="nav-item ">
                             <a href="#Inicio" class="nav-link text-light">Inicio</a>
                        </li>
                        <li class="nav-item">
                            <a href="#services" class="nav-link text-light">Servicios</a>
                        </li>
                        <li class="nav-item">
                            <a href="#news" class="nav-link text-light">Noticias</a>
                        </li>
                        <li class="nav-item">
                            <a href="#team" class="nav-link text-light">Equipo</a>
                        </li>
                    </ul>
                </div>                            
            </div>

 <div id="carouselExampleCaptions" class="carousel slide col-md-12 mt-3" data-ride="carousel" style="height: 300px;">
                <ol class="carousel-indicators" >
                  <li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
                  <li data-target="#carouselExampleCaptions" data-slide-to="1"></li>
                  <li data-target="#carouselExampleCaptions" data-slide-to="2"></li>
                </ol>
                <div class="carousel-inner">
                  <div class="carousel-item active">
                    <img src="Aprender.png" class="img-fluid" style="height: 300px;" alt="...">
                    <div class="carousel-caption d-none d-md-block">
                      <h5>BIENVENIDOS</h5>
                      <p>TODO SOBRE EL DEPORTE.</p>
                    </div>
                  </div>
                  <div class="carousel-item">
                    <img src="Aprender.png" class="img-fluid" style="height: 300px;" alt="...">
                    <div class="carousel-caption d-none d-md-block">
                      <h5>PAGINA</h5>
                      <p>TODO SOBRE EL DEPORTE.</p>
                    </div>
                  </div>
                  <div class="carousel-item">
                    <img src="Aprender.png" class="img-fluid" style="height: 300px;" alt="...">
                    <div class="carousel-caption d-none d-md-block">
                      <h5>DEPORTIVA</h5>
                      <p>TODO SOBRE EL DEPORTE.</p>
                    </div>
                  </div>
                </div>
                <a class="carousel-control-prev" href="#carouselExampleCaptions" role="button" data-slide="prev">
                  <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                  <span class="sr-only">Previous</span>
                </a>
                <a class="carousel-control-next" href="#carouselExampleCaptions" role="button" data-slide="next">
                  <span class="carousel-control-next-icon" aria-hidden="true"></span>
                  <span class="sr-only">Next</span>
                </a>
              </div>
</div>
</template>
<script>
export default {
  name: "EncabezadoPage",
};
</script>