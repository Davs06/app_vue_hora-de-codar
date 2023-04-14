<template>
  <div>
    <h1>Hello guys!!</h1>

    <p>My name is {{ nome }}, and my job is {{ job }}</p>

    <MultiplosEventos/>
  </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue'

export default {
  name: "primeiroComponente",
  components: {
    MultiplosEventos
  },
  data() {
    return {
      nome: "Davs",
      job: 'Dev Front-End'
    };
  },
};
</script>