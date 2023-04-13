<template>
  <div>
    <p v-if="in_job">Estou trabalhando no momento.</p>
    <p v-else>Estou me busca de novas oportunidades</p>

    <p>Ultilizo as seguintes tecnologias:</p>

    <ul>
      <li>JavaScript</li>
      <li>Java</li>
      <li>PHP</li>
    </ul>

    <div>
      <button @click="showEmail">{{ txt_btn }}</button>
    </div>

    <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
    <p>
      Para acessar meu portifolio,
      <a v-bind:href="meu_portifolio" target="_blank">basta clicar aqui </a>
    </p>
    <!-- Usar v-bind para links de outras pag-->
    <p>
      Para acessar meu github,
      <a v-bind:href="meu_github" target="_blank">basta clicar aqui </a>
    </p>
    <!-- Usar v-bind para links de outras pag-->

    <Picture />
  </div>
</template>

<script>
import Picture from "./Picture.vue";

export default {
  name: "InfoPessoa",
  components: {
    Picture,
  },
  data() {
    return {
      in_job: false,
      email: "davs@emai.com",
      mostrar_email: false,
      meu_portifolio: "https://portifolio-davs.netlify.app",
      meu_github: "https://github.com/Davs06",
      txt_btn: "Mostrar email",
    };
  },
  methods: {
    showEmail() {
      this.mostrar_email = !this.mostrar_email;

      if (!this.mostrar_email) {
        this.txt_btn = "Mostrar email";
      } else {
        this.txt_btn = "Esconder email";
      }
    },
  },
};
</script>