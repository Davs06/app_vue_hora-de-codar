<template>
  <div>
    <Picture />
    <p v-if="in_job">Estou trabalhando no momento.</p>
    <p v-else>Estou me busca de novas oportunidades</p>

    <p>Ultilizo as seguintes tecnologias para Back-End:</p>

    <ul>
      <li v-for="(technology, index) in technologiesFront" :key="index">
        {{ technology }}
      </li>
    </ul>

    <p>Ultilizo as seguinter tecnologias para Front-End</p>

    <ul>
      <li v-for="technology in technologiesBack" :key="technology.id">
        {{ technology.language }}
      </li>
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
      technologiesFront: ["Java", "PHP", "Node"],
      technologiesBack: [
        { id: 1, language: "HTML" },
        { id: 2, language: "CSS" },
        { id: 3, language: "JavaScript" },
        { id: 4, language: "Vue3" },
      ],
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