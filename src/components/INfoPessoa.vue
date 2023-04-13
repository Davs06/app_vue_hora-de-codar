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

    <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
  </div>
</template>

<script>
export default {
  name: "InfoPessoa",
  data() {
    return {
      in_job: false,
      email: "davs@emai.com",
      mostrar_email: true,
    };
  },
};
</script>