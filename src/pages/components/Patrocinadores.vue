<template>
  <div class="section" id="carousel">
    <div class="container">
      <div class="title">
        <h4>PATROCINADORES</h4>
      </div>
      <div class="row justify-content-center">
        <div class="col-8">
          <el-carousel height="115px">
            <el-carousel-item>
              <img class="d-block" src="patrocinio/aurora.jpg" alt="Ótica Aurora" />
            </el-carousel-item>
            <el-carousel-item>
              <img class="d-block" src="patrocinio/bkr.jpg" alt="BKR Eventos e Festas" />
            </el-carousel-item>
            <el-carousel-item>
              <img class="d-block" src="patrocinio/mantac.jpg" alt="Mantac" />
            </el-carousel-item>
            <el-carousel-item>
              <img class="d-block" src="patrocinio/digisom.png" alt="DigSom Aparelhos Auditivos" />
            </el-carousel-item>
            <el-carousel-item>
              <img class="d-block" src="patrocinio/livraria.jpg" alt="Livraria Sagrado Coração de Jesus" />
            </el-carousel-item>
            <el-carousel-item>
              <img class="d-block" src="patrocinio/moraes.jpg" alt="Moraes Escapamentos" />
            </el-carousel-item>
            <el-carousel-item>
              <img class="d-block" src="patrocinio/placasnorte.jpg" alt="Placas Norte" />
            </el-carousel-item>
          </el-carousel>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { Carousel, CarouselItem } from 'element-ui';

export default {
  components: {
    [Carousel.name]: Carousel,
    [CarouselItem.name]: CarouselItem
  }
};
</script>
<style></style>
