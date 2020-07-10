<template>
  <navbar
    position="fixed"
    type="primary"
    :transparent="transparent"
    :color-on-scroll="colorOnScroll"
    menu-classes="ml-auto"
  >
    <template>
      <router-link v-popover:popover1 class="navbar-brand" to="/">Santuário SCJ</router-link>
      <el-popover
        ref="popover1"
        popper-class="popover"
        placement="bottom"
        width="200"
        trigger="hover"
      >
        <div class="popover-body">Início</div>
      </el-popover>
    </template>
    <template slot="navbar-menu">
      <drop-down tag="li" title="Institucional" icon="now-ui-icons travel_istanbul" class="nav-item">
        <nav-link to="/institucional">
          <i class="now-ui-icons business_chart-pie-36"></i> Nossa História 
        </nav-link>
        <nav-link to="/agenda">
          <i class="now-ui-icons design_bullet-list-67"></i> Dehonianos 
        </nav-link>
        <nav-link to="/agenda">
          <i class="now-ui-icons design_bullet-list-67"></i> Seja um dizimista 
        </nav-link>
        <nav-link to="/agenda">
          <i class="now-ui-icons design_bullet-list-67"></i> Pastorais e Movimentos
        </nav-link>
        <nav-link to="/agenda">
          <i class="now-ui-icons business_chart-pie-36"></i> Espiritualidade 
        </nav-link>
        <nav-link to="/agenda">
          <i class="now-ui-icons design_bullet-list-67"></i> Clero 
        </nav-link>
        <nav-link to="/agenda">
          <i class="now-ui-icons business_chart-pie-36"></i> Horários 
        </nav-link>
      </drop-down>
      <drop-down tag="li" title="Notícias" icon="now-ui-icons design_app" class="nav-item">
        <nav-link to="/noticias">
          <i class="now-ui-icons education_paper"></i> Notícias da Paróquia
        </nav-link>
        <nav-link to="/noticias">
          <i class="now-ui-icons users_circle-08"></i> Notícias em Geral
        </nav-link>
        <nav-link to="/noticias">
          <i class="now-ui-icons users_single-02"></i> Artigos
        </nav-link>
      </drop-down>
      <li class="nav-item">
        <router-link class="nav-link" to="/multimidia">
          <i class="now-ui-icons media-1_camera-compact"></i>
          <p class="atalho">Multimídia</p>
        </router-link>
      </li>
      <drop-down tag="li" title="Interatividade" icon="now-ui-icons design_image" class="nav-item">
        <nav-link to="/agenda">
          <i class="now-ui-icons business_chart-pie-36"></i> Agenda
        </nav-link>
        <nav-link to="/agenda">
          <i class="now-ui-icons design_bullet-list-67"></i> Galeria de fotos
        </nav-link>
        <nav-link to="/agenda">
          <i class="now-ui-icons business_chart-pie-36"></i> Intenções
        </nav-link>
        <nav-link to="/agenda">
          <i class="now-ui-icons design_bullet-list-67"></i> Pedidos de oração
        </nav-link>
        <nav-link to="/agenda">
          <i class="now-ui-icons business_chart-pie-36"></i> Liturgia diária
        </nav-link>
        <nav-link to="/agenda">
          <i class="now-ui-icons design_bullet-list-67"></i> Santo do dia
        </nav-link>
      </drop-down>
      <drop-down tag="li" title="Contato" icon="now-ui-icons design_app" class="nav-item">
        <nav-link to="/landing">
          <i class="now-ui-icons education_paper"></i> Fale conosco
        </nav-link>
        <nav-link to="/login">
          <i class="now-ui-icons users_circle-08"></i> Horários
        </nav-link>
        <nav-link to="/profile">
          <i class="now-ui-icons users_single-02"></i> Localização
        </nav-link>
      </drop-down>

      <li class="nav-item">
        <a
          class="nav-link"
          rel="tooltip"
          title="Siga-nos no Instagram"
          data-placement="bottom"
          href="https://www.instagram.com/santuarioscj/"
          target="_blank"
        >
          <i class="fab fa-instagram"></i>
          <p class="d-lg-none d-xl-none">Instagram</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          rel="tooltip"
          title="Curta-nos no Facebook"
          data-placement="bottom"
          href="https://www.facebook.com/santuarioscj"
          target="_blank"
        >
          <i class="fab fa-facebook-square"></i>
          <p class="d-lg-none d-xl-none">Facebook</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          rel="tooltip"
          title="Inscreva-se em nosso canal no YouTube"
          data-placement="bottom"
          href="https://www.youtube.com/channel/UC2f7ehxyVDflfl0woFYGF3w/"
          target="_blank"
        >
          <i class="fab fa-youtube"></i>
          <p class="d-lg-none d-xl-none">YouTube</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          rel="tooltip"
          title="Siga-nos no Twitter"
          data-placement="bottom"
          href="https://twitter.com/santuarioscj"
          target="_blank"
        >
          <i class="fab fa-twitter"></i>
          <p class="d-lg-none d-xl-none">Twitter</p>
        </a>
      </li>
    </template>
  </navbar>
</template>

<script>
import { DropDown, Navbar, NavLink } from "@/components";
import { Popover } from "element-ui";
export default {
  name: "main-navbar",
  props: {
    transparent: Boolean,
    colorOnScroll: Number
  },
  components: {
    DropDown,
    Navbar,
    NavLink,
    [Popover.name]: Popover
  }
};
</script>

<style scoped>
.icone{
  font-size: 0.95rem;
}
.atalho{
  margin-left: 3px;
}
</style>
