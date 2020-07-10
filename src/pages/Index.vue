<template>
  <div>
    <div class="page-header clear-filter" filter-color="orange">
      <parallax class="page-header-image" style="background-image:url('img/header.jpg')"></parallax>
      <div class="container">
        <div class="content-center brand">
          <img class="n-logo" src="img/sscj-logo.png" alt />
          <h2 class="h1-seo">Santuário Sagrado Coração de Jesus</h2>
        </div>
      </div>
    </div>
    <div class="main">
    </div>
    <patrocinadores></patrocinadores>
    <novidades></novidades>
  </div>
</template>
<script>
import { Parallax } from "@/components";
import Patrocinadores from "./components/Patrocinadores";
import Novidades from "./components/Novidades";

export default {
  name: "index",
  bodyClass: "index-page",
  components: {
    Parallax,
    Patrocinadores,
    Novidades
  }
};
</script>
<style scoped>
</style>
