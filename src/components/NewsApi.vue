<template>
  <div>
    <div class="row mt-md-5 mt-sm-5 mt-xs-5">
      <div class="col-lg-6 col-xs-12" v-for="article in news" :key="article">
        <div class="d-flex justify-content-center align-items-center">
          <div class="p-3">
            <img :src="article.image" alt="Article Name" height="200px" width = "200px">
          </div>


          <div class="p-2">
              <h2>{{ article.title }}</h2>
                <hr>
            <p>
              {{ article.description }}
            </p>
          </div>
        </div>
        <div class="d-flex container-fluid justify-content-end pb-2 mt-n2">
          <a :href="article.url" class="btn btn-outline-info" >Info</a>
        </div>
      </div>
    </div>
  </div>
</template>




<script>
import axios from "axios";

export default {
  name: "NewsApi",
  data() {
    return {
      news: null,
    };
  },
  mounted() {
    axios
      .get(
        "https://gnews.io/api/v4/top-headlines?&topic=science&max=4&lang=es&token=6ace8181fd09ff2352f98ac3e6a80f92"
      )
      .then((response) => {
        this.news = response.data.articles;
        console.log(this.news[0].image);
      });
  },
};
</script>

<style lang="stylus" scoped></style>
