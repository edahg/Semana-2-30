<template>
  <div id="app">
    <div class="container-fluid">      
          <news-api></news-api>
        </div>
      </div>
    
</template>

<script>
import NewsApi from "./components/NewsApi.vue";

export default {
  name: "App",
  components: {
    NewsApi,
  },
  data() {
    return {
      title: "Vivo dentro de VUE",
    };
  },
};
</script>

