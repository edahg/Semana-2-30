<template>
  <div id="app">
    <div class="container-fluid">
      <news-api></news-api>
      <div class="row justify-content-center mb-5">
        <div class="col mt-5" v-for="member in team" :key="member">
          <team-card :member="member"></team-card>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import NewsApi from "./components/NewsApi.vue";
import TeamCard from './components/TeamCard.vue';


export default {
  name: "App",
  components: {
    NewsApi,
    TeamCard
  },
  data() {
    return { 
      team : [
        {
          codigo: 1,
          nombre: 'Edwin Gelacio',
          descripcion: 'Ingeniero de Software',
          rol: 'Scrum Master',
          image: 'https://cdn.iconscout.com/icon/free/png-256/avatar-380-456332.png'
        },
        {
          codigo: 2,
          nombre: 'Camila Suárez',
          descripcion: 'Ingeniera Quìmica Universidad de los Andes',
          rol: 'Frontend Developer',
          image: 'https://cdn.iconscout.com/icon/free/png-256/avatar-373-456325.png'
        },
        {
          codigo: 3,
          nombre: 'Alejandro Quintero',
          descripcion: 'Ingeniero electrónico y desarrollador de software',
          rol: 'Tester',
          image: 'https://cdn.iconscout.com/icon/free/png-256/avatar-372-456324.png'
        },
        {
          codigo: 4,
          nombre: 'Edgar Hoyos',
          descripcion: 'Ingeniero Electrónico Univalle',
          rol: 'Backend Developer',
          image: 'https://cdn.iconscout.com/icon/free/png-256/avatar-368-456320.png'
        }
      ]  
    } 
  }
};
</script>

