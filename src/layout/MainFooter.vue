<template>
  <footer
    class="footer"
    :class="{ [`footer-${type}`]: type }"
    :data-background-color="backgroundColor"
  >
    <div class="container caixa">
      <div class="util">
        <div class="titulo">CONTATO</div>
        <div
          class="blocos"
          data-scroll-reveal="enter from the left after 1.0s"
          data-scroll-reveal-initialized="true"
          data-scroll-reveal-complete="true"
        >
          <div class="dados">
            <div class="titulo1">Santuário Sagrado Coração de Jesus</div>
            <div class="localidade">
              Rua Inácio Bastos, 308 - Bucarein -
              <span>Joinville - SC</span>
            </div>
            <div class="telefones">
              <div class="telefone">(47) 3455-2204</div>
              <a
                href="https://web.whatsapp.com/send?1=pt_BR&amp;phone=5547991862335"
                target="_blank"
              >
                <div class="whats">(47) 9.9186-2335</div>
              </a>
            </div>
          </div>
        </div>
      </div>
      <div class="horarios">
        <div class="titulo2">HORÁRIO DE ATENDIMENTO</div>Segunda-feira:
        <span>fechada</span>
        <br />Terça a Sexta-feira
        <span>8h às 12h e 13h às 17h</span>
        <br />Sábado
        <span>8h às 12h</span>
      </div>
      <div class="copyright">
        &copy; {{ year }}, Desenvolvido por
        <a
          href="https:///www.invisionapp.com"
          target="_blank"
          rel="noopener"
        >MM Design</a>.
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    backgroundColor: String,
    type: String
  },
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>
<style scoped>
.caixa {
  display: flex;
  flex-direction: row;
  align-items: center;
}
.util {
  flex-grow: 1;
}
.horarios {
  flex-grow: 1;
}
.copyright {
  flex-grow: 1;
}
</style>
