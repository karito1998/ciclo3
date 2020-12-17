<template>
  <div id="app">
    <!--Seccion 4-->
    <div id= "team" class="container-fluid">
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
      descripcion : 'Ingeniera Electronica egresada de la universidad ECCI en Bogotá desarrolladora backend en mi.com.co, amante de los gatos, taekwondista.',
      rol: 'Analista de Software',
      image : './public/imagenes/KarolGisselleArciniegasMartinez.png'
      },
      {
      codigo : 2,
      nombre : 'Andres Sabogal',
      descripcion : 'Estudiante',
      rol: 'Desarrollador Frontend',
      image : './public/imagenes/AndresSabogal.png'
      },
      {
      codigo : 3,
      nombre : 'Deivier Zaraza',
      descripcion : 'Administrador financiero, con amplia experiencia en remodelaciones de espacios, emprendedor, autodidacta, apasionado por la musica, los viajes, los animales y el deporte.',
      rol: 'Arquitecto de software',
      image : './public/imagenes/DeivierZaraza.jpeg'
      },
    ]
    }
  }
  
}
</script>

