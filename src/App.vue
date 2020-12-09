<template>
  <div id="app" class="container bg-dark">
      <encabezado-page></encabezado-page>
      <seccion-servicios></seccion-servicios>
      <div class="text-light mt-2 mb-3 text-center">
          <h2>NOTICIAS</h2>
      </div>
      <div class="container">
        <seccion-noticias></seccion-noticias> 
      </div> 
      <div id="team" class="section-2 col-md-12 text-center pr-5 bg-secondary">
        <div class="text-light mt-2 mb-3">
          <h2>EQUIPO</h2>
        </div>
        <div class="row d-flex justify-content-between">
          <div class="col-md-3" v-for="(item,index) of team" :key="index">
              <team-card v-bind:member = "item"></team-card>
          </div>
        </div>
      </div>
      <page-footer></page-footer>    
  </div>
</template>

<script>
import PageFooter from './components/PageFooter.vue'
import TeamCard from './components/TeamCard.vue'
import SeccionNoticias from './components/SeccionNoticias.vue'
import SeccionServicios from './components/SeccionServicios.vue'
import EncabezadoPage from './components/EncabezadoPage.vue'

export default {
  name: 'App',
  components:{
    PageFooter,
    TeamCard,
    SeccionNoticias,
    SeccionServicios,
   EncabezadoPage,
  },
  data(){
    return{
      title:'Vivo dentro de VUE',
      team: [
        {
          codigo: 1,
          nombre: "Juan Francisco Pabón Caviativa",
          descripcion:
            "Ingeniero Electrónico (ITIL4) | Cine Lectura y Música | 37 Años",
          rol: "Desarrollador Backend - Tester",
          imagen: "Juan Pabón.png"
        },
        {
          codigo: 2,
          nombre: "Jesús David Rivas Losada",
          descripcion:
            "Estudiante de Ingeniería de Software | Cine, música y amigos | 27 Años",
          rol: "Desarrollador Front-END - Tester",
          imagen: "Jesús Rivas.png"
        },
        {
          codigo: 3,
          nombre: "Santiago Monsalve Botero",
          descripcion:
            "Estudiante de Diseño Visual &  Mercadeo y Publicidad | Lectura Música | 23 Años",
          rol: "Arquitecto de Software - Tester",
          imagen: "Santiago Monsalve (2).png"
        },
        {
          codigo: 4,
          nombre: "Esteban Madrid",
          descripcion:
            "Support Supervisor and Compliance & HR Associate | Gaming y Programación | 18 Años",
          rol: "Analista de Software - Tester",
          imagen: "Esteban Madrid.png"
        }
      ]
    }
  }
}
</script>

