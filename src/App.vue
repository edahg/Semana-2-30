<template>
  <div id="app">
    
      <top-banner></top-banner>
      <div class="container-fluid">
        <news-api></news-api>
      </div>
      <div class="row justify-content-center mb-5">
        <div class="col mt-5" v-for="member in team" :key="member">
          <team-card :member="member"></team-card>          
        </div>       
      </div>  
      <page-footer></page-footer>     
    </div>
    
</template>

<script>
import PageFooter from './components/PageFooter.vue';
import NewsApi from "./components/NewsApi.vue";
import TeamCard from './components/TeamCard.vue';
import TopBanner from './components/TopBanner.vue';
import TeamData from './assets/team.json'
  
export default {
  name: "App",
  components: {
    NewsApi,
    TeamCard,
    PageFooter,
    TopBanner
  },
  data() {
    return { 
        team : TeamData
    } 
  }
};
</script>

