<template>
  <div>
    <Reutilizacao />
    <h1>Hello guys!!</h1>
    <Reutilizacao />
    <Reutilizacao />

    <p>My name is {{ nome }}, and my job is {{ job }}</p>
    <Reutilizacao />

    <MultiplosEventos /><br /><br /><br />

    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
  </div>
</template>

<script>
import MultiplosEventos from "./MultiplosEventos.vue";
import Reutilizacao from "./Reutilizacao.vue";

export default {
  name: "primeiroComponente",
  components: {
    MultiplosEventos,
    Reutilizacao,
  },
  data() {
    return {
      nome: "Davs",
      job: "Dev Front-End",
    };
  },
};
</script>