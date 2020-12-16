<template>
  <div id="app">
    <!--Seccion 4-->
    <div class="container-fluid">
      <div class="row justify-content-center mb-5">
        <div class= "col mt-5" v-for="(miembro, index) of Team" :key = "index">
          <team-card :member="miembro"></team-card>

        </div>
       </div>
       </div> 
  </div>
</template>

<script>
import TeamCard from './components/TeamCard.vue'

export default {
  name: 'App',
  components: { TeamCard },
  data(){
    return{
    Team:[
      {
      codigo : 1,
      nombre : 'Karol Arciniegas',
      descripcion : 'Ingeniera Electronica egresada de la universidad ECCI en Bogota, amante de los gatos.',
      rol: 'Analista de Software',
      image : './public/imagenes/KarolGisselleArciniegasMartinez.png'
      },
      {
      codigo : 2,
      nombre : 'Andres Sabogal',
      descripcion : 'Ingeniera Electronica egresada de la universidad ECCI en Bogota, amante de los gatos.',
      rol: ' Desarrollador Backend',
      image : './public/imagenes/AndresSabogal.png'
      },
      {
      codigo : 3,
      nombre : 'Deivier Zaraza',
      descripcion : 'Ingeniera Electronica egresada de la universidad ECCI en Bogota, amante de los gatos.',
      rol: 'Arquitecto de software',
      image : './public/imagenes/DeivierZaraza.jpeg'
      },
    ]
    }
  }
  
}
</script>

