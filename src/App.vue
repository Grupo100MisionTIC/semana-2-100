<template>
  <div id="app">
    <div class="container-fluid">
      <div class="d-flex justify-content-center">
        <div class="col-12 col-md-2" v-for="(item, index) of gMembers" :key="index">
          <TeamCard v-bind:member="item"></TeamCard>      
        </div>
      </div>
    </div>    
    <page-footer> </page-footer>
  </div>
</template>

<script>

  import TeamCard from './components/TeamCard.vue';
  //import PageFooter from './components/PageFooter.vue';

export default {
  
  
    name: 'App',
    components: {
      TeamCard,
      PageFooter,
    },
    data(){
      return{
        gMembers: [
          {
              codigo: 1,
              nombre:"Julián Andrés García Rojas",
              descripcion:"Contador Público.",
              rol:"Desarrollador",
              imagen: "https://i.postimg.cc/xXWD8jQT/Julian.jpg"
          },

          {
              codigo: 2,
              nombre: "Juan Sebastian Prado Rodriguez",
              descripcion: "Ingeniero Ambiental.",
              rol: "Desarrollador",
              imagen: "https://i.postimg.cc/r0NvfSrK/Sebastian.jpg"
          },

          
          {
              codigo: 3,
              nombre: "Nicolás Garcés Sánchez",
              descripcion: "Ingeniero Químico.",
              rol: "Desarrollador",
              imagen: "https://i.postimg.cc/VSnyCys9/Nicolas.jpg"
          },

          {
              codigo: 4,
              nombre: "Jorge Daniel Quintero Galindo",
              descripcion: "Estudiante.",
              rol: "Desarrollador",
              imagen: "https://i.postimg.cc/Yv4BtGJs/Jorge-Daniel.jpg"
          },


          {
              codigo: 5,
              nombre: "Raúl Esteban Amaya Jiménez",
              descripcion: "Administrador.",
              rol: "Desarrollador",
              imagen: "https://i.postimg.cc/hzBk8Chk/Raul-Amaya.jpg"
          }

        ]
      }
    } 
}
</script>

