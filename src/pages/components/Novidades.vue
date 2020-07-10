<template>
  <div class="caixa">
    <card class="card-newsletter" header-classes="text-center" color="brown">
      <p class="botao">
        CADASTRE SEU E-MAIL
        E RECEBA NOVIDADES
      </p>
      <template>
        <fg-input
          class="no-border"
          placeholder="Nome"
          addon-left-icon="now-ui-icons users_circle-08"
        ></fg-input>

        <fg-input
          class="no-border"
          placeholder="E-mail"
          addon-left-icon="now-ui-icons ui-1_email-85"
        ></fg-input>
      </template>
      <div class="botao">
        <n-button type="neutral" round size="lg">Cadastrar</n-button>
      </div>
    </card>
  </div>
</template>

<script>
import { Card, FormGroupInput, Button } from "@/components";

export default {
  components: {
    Card,
    [Button.name]: Button,
    [FormGroupInput.name]: FormGroupInput
  }
};
</script>

<style scoped>
.caixa {
  display: -webkit-flex;
  display: flex;
  flex-direction: row wrap;
  justify-content: space-around;
  align-items: center;
}

.card-newsletter {
  width: 50%;
  border-radius: 20px;
  padding: 6px;
}
.botao {
  text-align: center;
}

@media screen and (max-width: 557px) {
  .card-newsletter {
    width: 100%;
    padding: 3px;
    border-radius: 10px;
  }
}
@media screen and (max-width: 767px) {
  .card-newsletter {
    width: 80%;
    padding: 5px;
    border-radius: 15px;
  }
}
@media screen and (max-width: 991px) {
  .card-newsletter {
    width: 70%;
    border-radius: 20px;
    padding: 6px;
  }
}
</style>
