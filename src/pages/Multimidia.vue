<template>
  <div>
    <div class="page-header clear-filter" filter-color="orange">
      <parallax class="page-header-image" style="background-image:url('img/bg1.jpg')"></parallax>
      <div class="container">
        <tabs type="primary" tabContentClasses="tab-subcategories" square centered class="row">
          <tab-pane>
            <span slot="label">
              <i class="now-ui-icons objects_umbrella-13"></i>Agenda
            </span>
            <p>{{tabText.p11}}</p>
            <p>{{tabText.p12}}</p>
          </tab-pane>
          <tab-pane>
            <span slot="label">
              <i class="now-ui-icons shopping_shop"></i>Galeria de fotos
            </span>
            <p>{{tabText.p21}}</p>
            <p>{{tabText.p22}}</p>
          </tab-pane>
          <tab-pane>
            <span slot="label">
              <i class="now-ui-icons ui-2_settings-90"></i>Intenções
            </span>
            <p>{{tabText.p31}}</p>
            <p>{{tabText.p32}}</p>
          </tab-pane>
          <tab-pane>
            <span slot="label">
              <i class="now-ui-icons objects_umbrella-13"></i>Pedidos de oração
            </span>
            <p>{{tabText.p11}}</p>
            <p>{{tabText.p12}}</p>
          </tab-pane>
          <tab-pane>
            <span slot="label">
              <i class="now-ui-icons shopping_shop"></i>Liturgia diária
            </span>
            <p>{{tabText.p21}}</p>
            <p>{{tabText.p22}}</p>
          </tab-pane>
          <tab-pane>
            <span slot="label">
              <i class="now-ui-icons ui-2_settings-90"></i>Santo do dia
            </span>
            <p>{{tabText.p31}}</p>
            <p>{{tabText.p32}}</p>
          </tab-pane>
        </tabs>
      </div>
    </div>
  </div>
</template>
<script>
import { Tabs, TabPane } from "@/components";

export default {
  name: "multimidia",
  bodyClass: "profile-page",
  data() {
    return {
      tabText: {
        p11: "...",
        p12: "...",
        p21: "...",
        p22: "...",
        p31: "...",
        p32: "..."
      }
    };
  },
  components: {
    Tabs,
    TabPane
  }
};
</script>
<style></style>
