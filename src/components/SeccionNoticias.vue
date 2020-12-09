<template>
<div>
  <div class="row mt-md-5 mt-sm-5 mt-xs-5">
    <div class="col-lg-6 col-xs-12"  v-for="(noticia,index) of noticias" :key="index">
      <div class="d-flex justify-content-center align-items-center">
        <div class="p-3s">
          <img :src="noticia.urlToImage" class="img-fluid" alt="noticia imagen">
        </div>
        <div class="p-2">
          <h4 class="text-danger">{{noticia.title}}</h4>
          <p class="text-white">{{noticia.description}}</p>
        </div>
      </div>
      <div class="d-flex container-fluid justify-content-end pb-2 mt-n2">
        <a :href="noticia.url" target="_blank" class="btn btn-primary">Noticia</a>
      </div>
    </div>
  </div>
</div>
</template>
<script>
import axios from "axios";

export default {
  name: "SeccionNoticias",
  data() {
    return {
      noticias: null,
    };
  },
  mounted() {
    axios
      .get(
        "http://newsapi.org/v2/top-headlines?country=co&category=sports&apiKey=819637c18241420fb41c51496098fbc7"
      )
      .then((response) => {
        this.noticias = response.data.articles.slice(0, 4);
        console.log(this.noticias);
      });
  },
};
</script>